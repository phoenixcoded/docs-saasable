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
  supabase: () => import('@/app/api/supabase/auth').then((mod) => mod.default as AuthProvider)
};

// Dynamically loads and returns the auth provider based on AUTH_PROVIDER.
export async function authProvider() {
  return await authProviderMapping[AUTH_PROVIDER]();
}
```
{% endcode %}



Below code defines a POST API route handler that dynamically invokes the appropriate login function based on the currently configured authentication provider.

{% code title="src\app\api\auth\login\route.ts" %}
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

For authentication, we have two distinct business logic implementations based on the selected `AUTH_PROVIDER`:

1. **Mock**: The mock authentication logic is defined in `src/app/api/mock/auth/index.ts`.

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

2. **Supabase**: The Supabase authentication logic is defined in `src/app/api/supabase/auth/index.ts`.

{% code title="src/app/api/supabase/auth/index.ts" %}
```typescript
// @next
import { NextResponse } from 'next/server';

export async function login(request: Request) {
  try {
    ...  // logic of supabase
  } catch {
    return NextResponse.json({ error: 'Server error' }, { status: 500 });
  }
}

...
```
{% endcode %}
