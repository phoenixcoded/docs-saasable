# Config

SaasAble admin uses a single source of truth for default configurations, allowing users to manage settings effectively and making it scalable for new configurations. You can configure options such as font, locale, and more in `src/config.ts`.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/config.ts" %}
```typescript
// @project
import { AuthType } from '@/enum';

// @types
import { ConfigProps } from '@/types/config';

/***************************  THEME CONSTANT  ***************************/

export const APP_DEFAULT_PATH = '/dashboard/analytics/overview';
export const APP_SUPPORT_PATH = 'https://phoenixcoded.authordesk.app/';

export const DRAWER_WIDTH = 254;
export const MINI_DRAWER_WIDTH = 76 + 1; // 1px - for right-side border

/***************************  AUTH CONSTANT  ***************************/

export const AUTH_USER_KEY = 'auth-user';
export const AUTH_PROVIDER: AuthType = AuthType.MOCK;

/***************************  THEME ENUM  ***************************/

export enum Themes {
  THEME_CRM = 'crm',
  THEME_AI = 'ai',
  THEME_HOSTING = 'hosting'
}

export enum ThemeMode {
  LIGHT = 'light',
  DARK = 'dark'
}

export enum ThemeDirection {
  LTR = 'ltr',
  RTL = 'rtl'
}

export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

export enum ThemeFonts {
  FONT_ROBOTO = `'Roboto', sans-serif`,
  FONT_ARCHIVO = `'Archivo', sans-serif`,
  FONT_FIGTREE = `'Figtree', sans-serif`
}

/***************************  CONFIG  ***************************/

const config: ConfigProps = {
  currentTheme: Themes.THEME_HOSTING,
  mode: ThemeMode.LIGHT,
  themeDirection: ThemeDirection.LTR,
  miniDrawer: false,
  i18n: ThemeI18n.EN
};

export default config;

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/config.js" %}
```javascript
// @project
import { AuthType } from '@/enum';

/***************************  THEME CONSTANT  ***************************/

export const APP_DEFAULT_PATH = '/dashboard/analytics/overview';
export const APP_SUPPORT_PATH = 'https://phoenixcoded.authordesk.app/';

export const DRAWER_WIDTH = 254;
export const MINI_DRAWER_WIDTH = 76 + 1; // 1px - for right-side border

/***************************  AUTH CONSTANT  ***************************/

export const AUTH_USER_KEY = 'auth-user';
export const AUTH_PROVIDER = AuthType.MOCK;

/***************************  THEME ENUM  ***************************/

export let Themes;

(function (Themes) {
  Themes['THEME_CRM'] = 'crm';
  Themes['THEME_AI'] = 'ai';
  Themes['THEME_HOSTING'] = 'hosting';
})(Themes || (Themes = {}));

export let ThemeMode;

(function (ThemeMode) {
  ThemeMode['LIGHT'] = 'light';
  ThemeMode['DARK'] = 'dark';
})(ThemeMode || (ThemeMode = {}));

export let ThemeDirection;

(function (ThemeDirection) {
  ThemeDirection['LTR'] = 'ltr';
  ThemeDirection['RTL'] = 'rtl';
})(ThemeDirection || (ThemeDirection = {}));

export let ThemeI18n;

(function (ThemeI18n) {
  ThemeI18n['EN'] = 'en';
  ThemeI18n['FR'] = 'fr';
  ThemeI18n['RO'] = 'ro';
  ThemeI18n['ZH'] = 'zh';
})(ThemeI18n || (ThemeI18n = {}));

export let ThemeFonts;

(function (ThemeFonts) {
  ThemeFonts['FONT_ROBOTO'] = "'Roboto', sans-serif";
  ThemeFonts['FONT_ARCHIVO'] = "'Archivo', sans-serif";
  ThemeFonts['FONT_FIGTREE'] = "'Figtree', sans-serif";
})(ThemeFonts || (ThemeFonts = {}));

/***************************  CONFIG  ***************************/

const config = {
  currentTheme: Themes.THEME_HOSTING,
  mode: ThemeMode.LIGHT,
  themeDirection: ThemeDirection.LTR,
  miniDrawer: false,
  i18n: ThemeI18n.EN
};

export default config;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/config.ts" %}
```typescript
// @next
import { Archivo, Figtree, Roboto } from 'next/font/google';

// @project
import { AuthType } from '@/enum';

// @types
import { ConfigProps } from '@/types/config';

/***************************  THEME CONSTANT  ***************************/

export const APP_DEFAULT_PATH = '/dashboard/analytics';
export const APP_SUPPORT_PATH = 'https://phoenixcoded.authordesk.app/';

export const DRAWER_WIDTH = 254;
export const MINI_DRAWER_WIDTH = 76 + 1; // 1px - for right-side border

/***************************  AUTH CONSTANT  ***************************/

export const AUTH_USER_KEY = 'auth-user';
export const AUTH_PROVIDER: AuthType = AuthType.MOCK;

/***************************  THEME ENUM  ***************************/

export enum Themes {
  THEME_CRM = 'crm',
  THEME_AI = 'ai',
  THEME_HOSTING = 'hosting'
}

export enum ThemeMode {
  LIGHT = 'light',
  DARK = 'dark'
}

export enum ThemeDirection {
  LTR = 'ltr',
  RTL = 'rtl'
}

export enum ThemeI18n {
  EN = 'en',
  FR = 'fr',
  RO = 'ro',
  ZH = 'zh'
}

/***************************  CONFIG  ***************************/

const config: ConfigProps = {
  currentTheme: Themes.THEME_HOSTING,
  mode: ThemeMode.LIGHT,
  themeDirection: ThemeDirection.LTR,
  miniDrawer: false,
  i18n: ThemeI18n.EN
};

export default config;

/***************************  THEME - FONT FAMILY  ***************************/

const fontRobot = Roboto({ subsets: ['latin'], display: 'swap', weight: ['100', '300', '400', '500', '700', '900'] });
const fontArchivo = Archivo({ subsets: ['latin'], display: 'swap', weight: ['400', '500', '600', '700'] });
const fontFigtree = Figtree({ subsets: ['latin'], display: 'swap', weight: ['400', '500', '600', '700'] });

export const FONT_ROBOTO: string = fontRobot.style.fontFamily;
export const FONT_ARCHIVO: string = fontArchivo.style.fontFamily;
export const FONT_FIGTREE: string = fontFigtree.style.fontFamily;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/config.js" %}
```javascript
// @next
import { Archivo, Figtree, Roboto } from 'next/font/google';

// @project
import { AuthType } from '@/enum';

/***************************  THEME CONSTANT  ***************************/

export const APP_DEFAULT_PATH = '/dashboard/analytics/overview';
export const APP_SUPPORT_PATH = 'https://phoenixcoded.authordesk.app/';

export const DRAWER_WIDTH = 254;
export const MINI_DRAWER_WIDTH = 76 + 1; // 1px - for right-side border

/***************************  AUTH CONSTANT  ***************************/

export const AUTH_USER_KEY = 'auth-user';
export const AUTH_PROVIDER = AuthType.MOCK;

/***************************  THEME ENUM  ***************************/

export let Themes;

(function (Themes) {
  Themes['THEME_CRM'] = 'crm';
  Themes['THEME_AI'] = 'ai';
  Themes['THEME_HOSTING'] = 'hosting';
})(Themes || (Themes = {}));

export let ThemeMode;

(function (ThemeMode) {
  ThemeMode['LIGHT'] = 'light';
  ThemeMode['DARK'] = 'dark';
})(ThemeMode || (ThemeMode = {}));

export let ThemeDirection;

(function (ThemeDirection) {
  ThemeDirection['LTR'] = 'ltr';
  ThemeDirection['RTL'] = 'rtl';
})(ThemeDirection || (ThemeDirection = {}));

export let ThemeI18n;

(function (ThemeI18n) {
  ThemeI18n['EN'] = 'en';
  ThemeI18n['FR'] = 'fr';
  ThemeI18n['RO'] = 'ro';
  ThemeI18n['ZH'] = 'zh';
})(ThemeI18n || (ThemeI18n = {}));

/***************************  CONFIG  ***************************/

const config = {
  currentTheme: Themes.THEME_HOSTING,
  mode: ThemeMode.LIGHT,
  themeDirection: ThemeDirection.LTR,
  miniDrawer: false,
  i18n: ThemeI18n.EN
};

export default config;

/***************************  THEME - FONT FAMILY  ***************************/

const fontRobot = Roboto({ subsets: ['latin'], display: 'swap', weight: ['100', '300', '400', '500', '700', '900'] });
const fontArchivo = Archivo({ subsets: ['latin'], display: 'swap', weight: ['400', '500', '600', '700'] });
const fontFigtree = Figtree({ subsets: ['latin'], display: 'swap', weight: ['400', '500', '600', '700'] });

export const FONT_ROBOTO = fontRobot.style.fontFamily;
export const FONT_ARCHIVO = fontArchivo.style.fontFamily;
export const FONT_FIGTREE = fontFigtree.style.fontFamily;

```
{% endcode %}
{% endtab %}
{% endtabs %}
