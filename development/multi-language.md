---
description: Localization support IE11, Edge, Chrome, Firefox & Safari.
---

# Multi Language

SassAble supports four languages ('en' - English, 'fr' - French, 'ro' - Romanian, 'zh' - Chinese) and can be easily switched from the header profile tab. The main menu is also internationalised for all four languages. If you wish to add a or set a default language, please continue reading below...

## How does it work?

Data for locale files exists at **`src\utils\locales`**

{% code title=".json file" %}
```json
{
  "manage": "Manage",
  "dashboard": "Dashboard",
  "home": "Home",
   ...
   ...
}
```
{% endcode %}

To change the Locale, open the file **`src\config`** file and set language

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src\config.ts"><code class="lang-typescript">...

// @types
import { ConfigProps } from '@/types/config';

<strong>...
</strong>
export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

/***************************  CONFIG  ***************************/

const config: ConfigProps = {
  ...
  i18n: ThemeI18n.EN
};

...
</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-typescript" data-title="src\config.js"><code class="lang-typescript">
<strong>...
</strong>
export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

/***************************  CONFIG  ***************************/

const config = {
  ...
  i18n: ThemeI18n.EN
};

...
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
<pre class="language-typescript" data-title="src\config.ts"><code class="lang-typescript">...

// @types
import { ConfigProps } from '@/types/config';

<strong>...
</strong>
export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

/***************************  CONFIG  ***************************/

const config: ConfigProps = {
  ...
  i18n: ThemeI18n.EN
};

...
</code></pre>
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src\config.js" %}
```javascript
...

export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

/***************************  CONFIG  ***************************/

const config = {
  ...
  i18n: ThemeI18n.EN
};

...
```
{% endcode %}
{% endtab %}
{% endtabs %}

Open file `src/app/ProviderWrapper`&#x20;

{% tabs %}
{% tab title="VITE(TS)" %}


<pre class="language-typescript" data-title="src/App.tsx"><code class="lang-typescript"><strong>import { RouterProvider } from 'react-router-dom';
</strong>
// @project
import Locales from '@/components/Locales';
import RTLLayout from '@/components/RTLLayout';
import Snackbar from '@/components/Snackbar';
import Notistack from '@/components/third-party/Notistack';
import { ConfigProvider } from '@/contexts/ConfigContext';

import Metrics from '@/metrics';
import router from '@/routes';
import ThemeCustomization from '@/themes';

function App() {
  return (
    &#x3C;>
      &#x3C;ConfigProvider>
        &#x3C;ThemeCustomization>
          &#x3C;RTLLayout>
            &#x3C;Locales>
              &#x3C;Notistack>
                &#x3C;RouterProvider router={router} />
                &#x3C;Snackbar />
              &#x3C;/Notistack>
            &#x3C;/Locales>
          &#x3C;/RTLLayout>
        &#x3C;/ThemeCustomization>
      &#x3C;/ConfigProvider>
      &#x3C;Metrics />
    &#x3C;/>
  );
}

export default App;

</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}


{% code title="src/App.jsx" %}
```javascript
import { RouterProvider } from 'react-router-dom';

// @project
import Locales from '@/components/Locales';
import RTLLayout from '@/components/RTLLayout';
import Snackbar from '@/components/Snackbar';
import Notistack from '@/components/third-party/Notistack';
import { ConfigProvider } from '@/contexts/ConfigContext';

import Metrics from '@/metrics';
import router from '@/routes';
import ThemeCustomization from '@/themes';

function App() {
  return (
    <>
      <ConfigProvider>
        <ThemeCustomization>
          <RTLLayout>
            <Locales>
              <Notistack>
                <RouterProvider router={router} />
                <Snackbar />
              </Notistack>
            </Locales>
          </RTLLayout>
        </ThemeCustomization>
      </ConfigProvider>
      <Metrics />
    </>
  );
}

export default App;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/ProviderWrapper.tsx" %}
```typescript
'use client';

// @project
import Locales from '@/components/Locales';
import RTLLayout from '@/components/RTLLayout';
import Snackbar from '@/components/Snackbar';
import Notistack from '@/components/third-party/Notistack';
import { ConfigProvider } from '@/contexts/ConfigContext';
import ThemeCustomization from '@/themes';

// @types
import { ChildrenProps } from '@/types/root';

/***************************  LAYOUT - CONFIG, THEME  ***************************/

export default function ProviderWrapper({ children }: ChildrenProps) {
  return (
    <ConfigProvider>
      <ThemeCustomization>
        <RTLLayout>
          <Notistack>
            <Snackbar />
            <Locales>{children}</Locales>
          </Notistack>
        </RTLLayout>
      </ThemeCustomization>
    </ConfigProvider>
  );
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/ProviderWrapper.jsx" %}
```javascript
'use client';

import PropTypes from 'prop-types';

// @project
import Locales from '@/components/Locales';
...

/***************************  LAYOUT - CONFIG, THEME  ***************************/

export default function ProviderWrapper({ children }) {
  return (
    ...
      <Locales>{children}</Locales>
    ...
  );
}

ProviderWrapper.propTypes = { children: PropTypes.any };
```
{% endcode %}
{% endtab %}
{% endtabs %}

## How to Use i18n in Any Custom Component?

This is the simplest and most common way to use translations in your components.

```typescript
import { FormattedMessage } from 'react-intl';

const MyComponent = () => {
  return (
    <div>
      <h2><FormattedMessage id="dashboard" /></h2>
      <p><FormattedMessage id="demo" /></p>
    </div>
  );
};

```

Update json file according FormattedMessage ID value.&#x20;

{% code title="en.json" %}
```json
{
  
  "dashboard": "Dashboard",
  "demo": "Demo",
   ...
   ...
}
```
{% endcode %}

{% code title="zh.json" %}
```json
{
   "dashboard": "仪表板",
   "demo": "演示",
   ...
   ...
}
```
{% endcode %}

{% code title="fr.json" %}
```json
{
   "dashboard": "Tableau de bord",
   "demo": "Démo",
   ...
   ...
}
```
{% endcode %}

{% code title="ro.json" %}
```json
{
   "dashboard": "Bord",
   "demo": "Demonstrație",
   ...
   ...
}
```
{% endcode %}
