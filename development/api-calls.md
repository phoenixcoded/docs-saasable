# API Calls

We've integrated Axios to handle API calls. By default, it uses the current host URL, but you can customize this in the `.env` file to suit your requirements.

{% code title=".env" %}
```properties
...
NEXT_PUBLIC_API_HOST=
...
```
{% endcode %}

Axios has been configured in the folder **`src/utils/axios.ts`**

### Auth api work scenario

We have our all API's in the **`src/app/api`** directory. In this directory, there is a folder named **`auth`**, which contains our authentication-related APIs.\
\
The **`AUTH_PROVIDER`** can be set to either **`mock`** or **`supabase`**. Both options utilize the same API endpoint, with the backend dynamically invoking the corresponding business logic based on the **`AUTH_PROVIDER`** configuration. \
\
The **`authProvider.ts`** file manages this distinction by dynamically loading and returning the appropriate authentication provider module.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/utils/api/auth/authProvider.ts" %}
```typescript
// @project
import { AUTH_PROVIDER } from '@/config';

export interface AuthProvider {
  login: (formData: Record<string, any>) => Promise<Response>;
  getUser: () => Promise<Response>;
  forgotPassword?: (formData: Record<string, any>) => Promise<Response>;
  resetPassword?: (formData: Record<string, any>) => Promise<Response>;
  signOut?: () => Promise<Response>;
  signUp?: (formData: Record<string, any>) => Promise<Response>;
  verifyOtp?: (formData: Record<string, any>) => Promise<Response>;
  resend?: (formData: Record<string, any>) => Promise<Response>;
}

// Mapping of auth types to dynamic imports
const authProviderMapping: Record<string, () => Promise<AuthProvider>> = {
  mock: () => import('@/utils/api/auth/mock/auth').then((mod) => mod.default as unknown as AuthProvider),
  supabase: () => import('@/utils/api/auth/supabase/auth').then((mod) => mod.default as unknown as AuthProvider),
  aws: () => import('@/utils/api/auth/aws/auth').then((mod) => mod.default as unknown as AuthProvider)
};

// Dynamically loads and returns the auth provider based on AUTH_PROVIDER.
export async function authProvider() {
  return await authProviderMapping[AUTH_PROVIDER]();
}

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/utils/api/auth/authProvider.js" %}
```javascript
// @project
import { AUTH_PROVIDER } from '@/config';

// Mapping of auth types to dynamic imports
const authProviderMapping = {
  mock: () => import('@/utils/api/auth/mock/auth').then((mod) => mod.default),
  supabase: () => import('@/utils/api/auth/supabase/auth').then((mod) => mod.default),
  aws: () => import('@/utils/api/auth/aws/auth').then((mod) => mod.default)
};

// Dynamically loads and returns the auth provider based on AUTH_PROVIDER.
export async function authProvider() {
  return await authProviderMapping[AUTH_PROVIDER]();
}

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/api/auth/authProvider.ts" %}
```typescript
// @project
import { AUTH_PROVIDER } from '@/config';

interface AuthProvider {
  login: (request: Request) => Promise<Response>;
  getUser: (requestOrToken: Request | string) => Promise<Response>;
  forgotPassword?: (request: Request) => Promise<Response>;
  resetPassword?: (request: Request) => Promise<Response>;
  signOut?: (request: Request) => Promise<Response>;
  signUp?: (request: Request) => Promise<Response>;
  verifyOtp?: (request: Request) => Promise<Response>;
  resend?: (request: Request) => Promise<Response>;
}

// Mapping of auth types to dynamic imports
const authProviderMapping: Record<string, () => Promise<AuthProvider>> = {
  mock: () => import('@/app/api/mock/auth').then((mod) => mod.default as AuthProvider),
  supabase: () => import('@/app/api/supabase/auth').then((mod) => mod.default as AuthProvider),
  aws: () => import('@/app/api/aws/auth').then((mod) => mod.default as AuthProvider)
};

// Dynamically loads and returns the auth provider based on AUTH_PROVIDER.
export async function authProvider() {
  return await authProviderMapping[AUTH_PROVIDER]();
}

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/api/auth/authProvider.js" %}
```javascript
// @project
import { AUTH_PROVIDER } from '@/config';

// Mapping of auth types to dynamic imports
const authProviderMapping = {
  mock: () => import('@/app/api/mock/auth').then((mod) => mod.default),
  supabase: () => import('@/app/api/supabase/auth').then((mod) => mod.default),
  aws: () => import('@/app/api/aws/auth').then((mod) => mod.default)
};

// Dynamically loads and returns the auth provider based on AUTH_PROVIDER.
export async function authProvider() {
  return await authProviderMapping[AUTH_PROVIDER]();
}
```
{% endcode %}
{% endtab %}
{% endtabs %}



The code below defines a POST API route handler that dynamically invokes the appropriate login function based on the currently configured authentication provider.

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src/utils/api/auth/index.ts"><code class="lang-typescript">// @project
import { authProvider } from './authProvider';
import { attempt } from '@/utils/attempt';

<strong>export async function login(formData: Record&#x3C;string, any>) {
</strong>  const authHandler = await authProvider();

  if (!authHandler.login) {
    return { data: null, error: 'Login not supported by current provider' };
  }

  return attempt(authHandler.login(formData));
}
</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/utils/api/auth/index.js" %}
```javascript
// @project
import { authProvider } from './authProvider';
import { attempt } from '@/utils/attempt';

export async function login(formData) {
  const authHandler = await authProvider();

  if (!authHandler.login) {
    return { data: null, error: 'Login not supported by current provider' };
  }

  return attempt(authHandler.login(formData));
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/api/auth/login/route.ts" %}
```typescript
// @next
import { NextResponse } from 'next/server';

// @project
import { authProvider } from '@/app/api/auth/authProvider';

export async function POST(request: Request) {
  try {
    const authProviderHandler = await authProvider();

    // Check if `login` is defined and is a function
    if (authProviderHandler.login) {
      return await authProviderHandler.login(request);
    } else {
      return NextResponse.json({ error: 'Login functionality not available' }, { status: 404 });
    }
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/api/auth/login/route.js" %}
```javascript
// @next
import { NextResponse } from 'next/server';

// @project
import { authProvider } from '@/app/api/auth/authProvider';

export async function POST(request) {
  try {
    const authProviderHandler = await authProvider();

    // Check if `login` is defined and is a function
    if (authProviderHandler.login) {
      return await authProviderHandler.login(request);
    } else {
      return NextResponse.json({ error: 'Login functionality not available' }, { status: 404 });
    }
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

```
{% endcode %}
{% endtab %}
{% endtabs %}

For authentication, we have two distinct business logic implementations based on the selected `AUTH_PROVIDER`:

1. **Mock**: The mock authentication logic is defined in `src/app/api/mock/auth/index.ts`.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/utils/api/auth/mock/auth/index.ts" %}
```typescript
export async function login(formData: LoginFormInput) {
  return new Promise((resolve, reject) => {
    try {
     ...  // logic of mock
    } catch {
      reject(new Error('Server error'));
    }
  });
}

...
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-javascript" data-title="src/utils/api/auth/mock/auth/index.js"><code class="lang-javascript"><strong>export async function login(formData) {
</strong>  return new Promise((resolve, reject) => {
    try {
    ... // logic of mock
    } catch {
      reject(new Error('Server error'));
    }
  });
}

...
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/api/mock/auth/index.ts" %}
```typescript
// @next
import { NextResponse } from 'next/server';

export async function login(request: Request) {
  try {
    ...  // logic of mock
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

...
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/api/mock/auth/index.js" %}
```javascript
// @next
import { NextResponse } from 'next/server';

export async function login(request) {
  try {
    ...  // logic of mock
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

...
```
{% endcode %}
{% endtab %}
{% endtabs %}

2. **Supabase**: The Supabase authentication logic is defined in `src/app/api/supabase/auth/index.ts`.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/utils/api/auth/supabase/auth/index.ts" %}
```typescript
export async function login(formData: LoginFormInput) {
  return new Promise(async (resolve, reject) => {
    try {
     ... // login of Supabase
    } catch {
      reject(new Error('Server error'));
    }
  });
}

... 
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/utils/api/auth/supabase/auth/index.js" %}
```javascript
export async function login(formData) {
  return new Promise(async (resolve, reject) => {
    try {
     ... // login of supabase
    } catch {
      reject(new Error('Server error'));
    }
  });
}

...
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/api/supabase/auth/index.ts" %}
```typescript
// @next
import { NextResponse } from 'next/server';

export async function login(request: Request) {
  try {
    ...  // login of supabase
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

...
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/api/supabase/auth/index.js" %}
```typescript
// @next
import { NextResponse } from 'next/server';

export async function login(request) {
  try {
    ...  // login of supabase
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

... 
```
{% endcode %}
{% endtab %}
{% endtabs %}
