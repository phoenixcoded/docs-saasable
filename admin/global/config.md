# Config

SaasAble admin uses a single source of truth for default configurations, allowing users to manage settings effectively and making it scalable for new configurations. You can configure options such as font, locale, and more in `src/config.ts`.

{% tabs %}
{% tab title="src/config.ts" %}
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
{% endtab %}
{% endtabs %}
