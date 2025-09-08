# Color

SaasAble admin with colors defined in the theme's palette. You can find these in the `palette.ts` file located in specific view folders. For instance, `src/themes/`.

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src/themes/palette.ts"><code class="lang-typescript">
/***************************  DEFAULT - PALETTE  ***************************/

export default function palette(mode: ThemeMode) {
  ...
  ...
  const lightPalette = {
    primary: {
      lighter: '#E0E0FF', // Hosting/primary/90 - primary container / primary fixed
      light: '#BDC2FF', // Hosting/primary/80 - primary fixed dim
      main: '#606BDF', // Hosting/primary/40 - primary
      dark: '#3944B8', // Hosting/primary/30 - on primary fixed variant
      darker: '#000668' // Hosting/primary/10 - on primary container / on primary fixed
    },
    ...
  };
<strong>
</strong>  const darkPalette = {
    primary: {
      lighter: '#2C37AC', // Hosting/primary/30 - primary container / on primary fixed variant
      light: '#7A86FB', // Hosting/primary/60 - primary fixed dim
      main: '#BDC2FF', // Hosting/primary/80 - primary
      dark: '#E0E0FF', // Hosting/primary/90 - on primary container / primary fixed
      darker: '#F1EFFF' // Hosting/primary/95 - on primary container / on primary fixed
    },
    ...
  };
  ...
}
</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-javascript" data-title="src/themes/palette.js"><code class="lang-javascript">
/***************************  DEFAULT - PALETTE  ***************************/

export default function palette(mode) {
  ...
  ...
  const lightPalette = {
    primary: {
      lighter: '#E0E0FF', // Hosting/primary/90 - primary container / primary fixed
      light: '#BDC2FF', // Hosting/primary/80 - primary fixed dim
      main: '#606BDF', // Hosting/primary/40 - primary
      dark: '#3944B8', // Hosting/primary/30 - on primary fixed variant
      darker: '#000668' // Hosting/primary/10 - on primary container / on primary fixed
    },
    ...
  };
<strong>
</strong>  const darkPalette = {
    primary: {
      lighter: '#2C37AC', // Hosting/primary/30 - primary container / on primary fixed variant
      light: '#7A86FB', // Hosting/primary/60 - primary fixed dim
      main: '#BDC2FF', // Hosting/primary/80 - primary
      dark: '#E0E0FF', // Hosting/primary/90 - on primary container / primary fixed
      darker: '#F1EFFF' // Hosting/primary/95 - on primary container / on primary fixed
    },
    ...
  };
  ...
}
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
<pre class="language-typescript" data-title="src/themes/palette.ts"><code class="lang-typescript">
/***************************  DEFAULT - PALETTE  ***************************/

export default function palette(mode: ThemeMode) {
  ...
  ...
  const lightPalette = {
    primary: {
      lighter: '#E0E0FF', // Hosting/primary/90 - primary container / primary fixed
      light: '#BDC2FF', // Hosting/primary/80 - primary fixed dim
      main: '#606BDF', // Hosting/primary/40 - primary
      dark: '#3944B8', // Hosting/primary/30 - on primary fixed variant
      darker: '#000668' // Hosting/primary/10 - on primary container / on primary fixed
    },
    ...
  };
<strong>
</strong>  const darkPalette = {
    primary: {
      lighter: '#2C37AC', // Hosting/primary/30 - primary container / on primary fixed variant
      light: '#7A86FB', // Hosting/primary/60 - primary fixed dim
      main: '#BDC2FF', // Hosting/primary/80 - primary
      dark: '#E0E0FF', // Hosting/primary/90 - on primary container / primary fixed
      darker: '#F1EFFF' // Hosting/primary/95 - on primary container / on primary fixed
    },
    ...
  };
  ...
}
</code></pre>
{% endtab %}

{% tab title="NEXT(JS)" %}
<pre class="language-javascript" data-title="src/themes/palette.js"><code class="lang-javascript">
/***************************  DEFAULT - PALETTE  ***************************/

export default function palette(mode) {
  ...
  ...
  const lightPalette = {
    primary: {
      lighter: '#E0E0FF', // Hosting/primary/90 - primary container / primary fixed
      light: '#BDC2FF', // Hosting/primary/80 - primary fixed dim
      main: '#606BDF', // Hosting/primary/40 - primary
      dark: '#3944B8', // Hosting/primary/30 - on primary fixed variant
      darker: '#000668' // Hosting/primary/10 - on primary container / on primary fixed
    },
    ...
  };
<strong>
</strong>  const darkPalette = {
    primary: {
      lighter: '#2C37AC', // Hosting/primary/30 - primary container / on primary fixed variant
      light: '#7A86FB', // Hosting/primary/60 - primary fixed dim
      main: '#BDC2FF', // Hosting/primary/80 - primary
      dark: '#E0E0FF', // Hosting/primary/90 - on primary container / primary fixed
      darker: '#F1EFFF' // Hosting/primary/95 - on primary container / on primary fixed
    },
    ...
  };
  ...
}
</code></pre>
{% endtab %}
{% endtabs %}

The details below contain the theme. for more information check [color page](https://admin.saasable.io/utils/color)

### Light mode color

#### 🎨 Primary color&#x20;

<table><thead><tr><th width="356">Name</th><th width="222">Variable name</th><th width="166">Color</th></tr></thead><tbody><tr><td>primary - <strong>Hosting/primary/40</strong></td><td>primary.main</td><td> #606BDF</td></tr><tr><td>primary container / primary fixed - <strong>Hosting/primary/90</strong></td><td>primary.lighter</td><td>#E0E0FF </td></tr><tr><td>primary fixed dim - <strong>Hosting/primary/80</strong></td><td>primary.light</td><td>#BDC2FF</td></tr><tr><td>on primary fixed variant - <strong>Hosting/primary/30</strong></td><td>primary.dark</td><td>#3944B8</td></tr><tr><td>on primary container / on primary fixed - <strong>Hosting/primary/10</strong></td><td>primary.darker</td><td>#000668</td></tr></tbody></table>

#### 🎨 Secondary color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>secondary - <strong>Hosting/secondary/40</strong></td><td>secondary.main</td><td>#5A5C78</td></tr><tr><td>secondary container / secondary fixed - <strong>Hosting/secondary/90</strong></td><td>secondary.lighter</td><td>#E0E0FF</td></tr><tr><td>secondary fixed dim - <strong>Hosting/secondary/80</strong></td><td>secondary.light</td><td>#C3C4E4</td></tr><tr><td>on secondary fixed variant - <strong>Hosting/secondary/30</strong></td><td>secondary.dark</td><td>#43455F</td></tr><tr><td>on secondary container / on secondary fixed - <strong>Hosting/secondary/10</strong></td><td>secondary.darker</td><td>#171A31</td></tr></tbody></table>

#### 🎨 Error color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>error - <strong>error/40</strong></td><td>error.main</td><td>#DE3730</td></tr><tr><td>error container / error fixed - <strong>error/90</strong></td><td>error.lighter</td><td>#FFEDEA</td></tr><tr><td>error fixed dim - <strong>error/80</strong></td><td>error.light</td><td>#FFDAD6</td></tr><tr><td>on error fixed variant - <strong>error/30</strong></td><td>error.dark</td><td>#BA1A1A</td></tr><tr><td>on error container / on error fixed - <strong>error/10</strong></td><td>error.darker</td><td>#690005</td></tr></tbody></table>

#### 🎨 Warning color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>warning - <strong>warning/40</strong></td><td>warning.main</td><td>#AE6600</td></tr><tr><td>warning container / warning fixed - <strong>warning/90</strong></td><td>warning.lighter</td><td>#FFEEE1</td></tr><tr><td>warning fixed dim - <strong>warning/80</strong></td><td>warning.light</td><td>#FFDCBE</td></tr><tr><td>on warning fixed variant - <strong>warning/30</strong></td><td>warning.dark</td><td>#8B5000</td></tr><tr><td>on warning container / on warning fixed - <strong>warning/10</strong></td><td>warning.darker</td><td>#4A2800</td></tr></tbody></table>

#### 🎨 Success color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>success - <strong>success/40</strong></td><td>success.main</td><td>#22892F</td></tr><tr><td>success container / success fixed - <strong>success/90</strong></td><td>success.lighter</td><td>#C8FFC0</td></tr><tr><td>success fixed dim - <strong>success/80</strong></td><td>success.light</td><td>#B6F2AF</td></tr><tr><td>on success fixed variant - <strong>success/30</strong></td><td>success.dark</td><td>#006E1C</td></tr><tr><td>on success container / on success fixed - <strong>success/10</strong></td><td>success.darker</td><td>#00390A</td></tr></tbody></table>

#### 🎨 Info color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>info - <strong>info/40</strong></td><td>info.main</td><td>#008394</td></tr><tr><td>info container / info fixed - <strong>info/90</strong></td><td>info.lighter</td><td>#D4F7FF</td></tr><tr><td>info fixed dim - <strong>info/80</strong></td><td>info.light</td><td>#A1EFFF</td></tr><tr><td>on info fixed variant - <strong>info/30</strong></td><td>info.dark</td><td>#006876</td></tr><tr><td>on info container / on info fixed - <strong>info/10</strong></td><td>info.darker</td><td>#00363E</td></tr></tbody></table>

#### 🎨 Grey color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface / surface bright - <strong>Hosting/neutral/98</strong></td><td>grey.50</td><td>#FBF8FF</td></tr><tr><td> surface container low - <strong>Hosting/neutral/96</strong></td><td>grey.100</td><td>#F5F2FA</td></tr><tr><td> surface container - <strong>Hosting/neutral/94</strong></td><td>grey.200</td><td>#EFEDF4</td></tr><tr><td> surface container high - <strong>Hosting/neutral/92</strong></td><td>grey.300</td><td>#EAE7EF</td></tr><tr><td>surface container highest - <strong>Hosting/neutral/90</strong></td><td>grey.400</td><td>#E4E1E6</td></tr><tr><td>surface dim - <strong>Hosting/neutral/87</strong></td><td>grey.500</td><td>#DBD9E0</td></tr><tr><td>outline variant - <strong>Hosting/neutral variant/80</strong></td><td>grey.600</td><td>#C7C5D0</td></tr><tr><td>outline - <strong>Hosting/neutral variant/50</strong></td><td>grey.700</td><td>#777680</td></tr><tr><td>on surface variant - <strong>Hosting/neutral variant/30</strong></td><td>grey.800</td><td>#46464F</td></tr><tr><td>on surface - <strong>Hosting/neutral/10</strong></td><td>grey.900</td><td>#1B1B1F</td></tr></tbody></table>

#### 🎨 Text color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>on surface - <strong>Hosting/neutral/10</strong></td><td>text.primary</td><td>#1B1B1F</td></tr><tr><td>on surface variant - <strong>Hosting/neutral variant/30</strong></td><td>text.secondary</td><td>#46464F</td></tr><tr><td>disabled color</td><td>text.disabled</td><td>#777680</td></tr></tbody></table>

#### 🎨 Common color

<table><thead><tr><th width="339">Name</th><th width="204">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface container - <strong>Hosting/neutral/94</strong></td><td>divider</td><td>#EFEDF4</td></tr><tr><td>white color </td><td>background.default</td><td>#FFF</td></tr><tr><td>secondary - <strong>Hosting/secondary/40</strong></td><td>action.hover</td><td>alpha(#5A5C78, 0.05)</td></tr><tr><td> outline - <strong>Hosting/neutral variant/50</strong></td><td>action.disabled</td><td>alpha(#777680, 0.6)</td></tr><tr><td>surface container highest - <strong>Hosting/neutral/90</strong></td><td>action.disabledBackground</td><td>alpha(#E4E1E6, 0.9)</td></tr></tbody></table>

### Dark mode color

#### 🎨 Primary color&#x20;

<table><thead><tr><th width="356">Name</th><th width="222">Variable name</th><th width="166">Color</th></tr></thead><tbody><tr><td>primary - <strong>Hosting/primary/80</strong></td><td>primary.main</td><td> #BDC2FF</td></tr><tr><td>primary container / on primary fixed variant - <strong>Hosting/primary/30</strong></td><td>primary.lighter</td><td>#2C37AC </td></tr><tr><td>primary fixed dim - <strong>Hosting/primary/60</strong></td><td>primary.light</td><td>#7A86FB</td></tr><tr><td>on primary container / primary fixed - <strong>Hosting/primary/90</strong></td><td>primary.dark</td><td>#E0E0FF</td></tr><tr><td>on primary container / on primary fixed - <strong>Hosting/primary/95</strong></td><td>primary.darker</td><td>#F1EFFF</td></tr></tbody></table>

#### 🎨 Secondary color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>secondary - <strong>Hosting/secondary/80</strong></td><td>secondary.main</td><td>#C3C4E4</td></tr><tr><td>secondary container / on secondary fixed variant - <strong>Hosting/secondary/30</strong></td><td>secondary.lighter</td><td>#43455F</td></tr><tr><td>secondary fixed dim - <strong>Hosting/secondary/60</strong></td><td>secondary.light</td><td>#8D8EAC</td></tr><tr><td>on secondary container / secondary fixed - <strong>Hosting/secondary/90</strong></td><td>secondary.dark</td><td>#E0E0FF</td></tr><tr><td>on secondary container / on secondary fixed - <strong>Hosting/secondary/95</strong></td><td>secondary.darker</td><td>#F1EFFF</td></tr></tbody></table>

#### 🎨 Error color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>error - <strong>error/80</strong></td><td>error.main</td><td>#FFDAD6</td></tr><tr><td>error container / on error fixed variant - <strong>error/30</strong></td><td>error.lighter</td><td>#BA1A1A</td></tr><tr><td>error fixed dim - <strong>error/60</strong></td><td>error.light</td><td>#FF897D</td></tr><tr><td>on error container / error fixed - <strong>error/90</strong></td><td>error.dark</td><td>#FFEDEA</td></tr><tr><td>on error container / on error fixed - <strong>error/95</strong></td><td>error.darker</td><td>#FFF8F7</td></tr></tbody></table>

#### 🎨 Warning color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>warning - <strong>warning/80</strong></td><td>warning.main</td><td>#FFDCBE</td></tr><tr><td>warning container / on warning fixed variant - <strong>warning/30</strong></td><td>warning.lighter</td><td>#8B5000</td></tr><tr><td>warning fixed dim - <strong>warning/60</strong></td><td>warning.light</td><td>#F79300</td></tr><tr><td>on warning container / warning fixed - <strong>warning/90</strong></td><td>warning.dark</td><td>#FFEEE1</td></tr><tr><td>on warning container / on warning fixed - <strong>warning/95</strong></td><td>warning.darker</td><td>#FFF8F5</td></tr></tbody></table>

#### 🎨 Success color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>success - <strong>success/80</strong></td><td>success.main</td><td>#B6F2AF</td></tr><tr><td>success container / on success fixed variant - <strong>success/30</strong></td><td>success.lighter</td><td>#006E1C</td></tr><tr><td>success fixed dim - <strong>success/60</strong></td><td>success.light</td><td>#5DC05E</td></tr><tr><td>on success container / success fixed - <strong>success/90</strong></td><td>success.dark</td><td>#C8FFC0</td></tr><tr><td>on success container / on success fixed - <strong>success/95</strong></td><td>success.darker</td><td>#ECFFE4</td></tr></tbody></table>

#### 🎨 Info color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>info - <strong>info/80</strong></td><td>info.main</td><td>#A1EFFF</td></tr><tr><td>info container / on info fixed variant - <strong>info/30</strong></td><td>info.lighter</td><td>#006876</td></tr><tr><td>info fixed dim - <strong>info/60</strong></td><td>info.light</td><td>#00BCD4</td></tr><tr><td>on info container / info fixed - <strong>info/90</strong></td><td>info.dark</td><td>#D4F7FF</td></tr><tr><td>on info container / on info fixed - <strong>info/95</strong></td><td>info.darker</td><td>#EEFCFF</td></tr></tbody></table>

#### 🎨 Grey color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface / surface dim - <strong>Hosting/neutral/06</strong></td><td>grey.50</td><td>#141218</td></tr><tr><td> surface container low - <strong>Hosting/neutral/10</strong></td><td>grey.100</td><td>#1B1B1F</td></tr><tr><td> surface container - <strong>Hosting/neutral/12</strong></td><td>grey.200</td><td>#211F26</td></tr><tr><td> surface container high - <strong>Hosting/neutral/17</strong></td><td>grey.300</td><td>#2B2930</td></tr><tr><td>surface container highest - <strong>Hosting/neutral/22</strong></td><td>grey.400</td><td>#36343B</td></tr><tr><td>surface container lowest - <strong>Hosting/neutral/04</strong></td><td>grey.500</td><td>#0F0D13</td></tr><tr><td>outline variant - <strong>Hosting/neutral variant/30</strong></td><td>grey.600</td><td>#46464F</td></tr><tr><td>outline - <strong>Hosting/neutral variant/60</strong></td><td>grey.700</td><td>#91909A</td></tr><tr><td>on surface variant - <strong>Hosting/neutral variant/80</strong></td><td>grey.800</td><td>#C7C5D0</td></tr><tr><td>on surface - <strong>Hosting/neutral/90</strong></td><td>grey.900</td><td>#E4E1E6</td></tr></tbody></table>

#### 🎨 Text color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>on surface - <strong>Hosting/neutral/90</strong></td><td>text.primary</td><td>#E4E1E6</td></tr><tr><td>on surface variant - <strong>Hosting/neutral variant/80</strong></td><td>text.secondary</td><td>#C7C5D0</td></tr><tr><td>outline - <strong>Hosting/neutral variant/60</strong></td><td>text.disabled</td><td>#91909A</td></tr></tbody></table>

#### 🎨 Common color

<table><thead><tr><th width="339">Name</th><th width="204">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface container - <strong>Hosting/neutral/12</strong></td><td>divider</td><td>#211F26</td></tr><tr><td>container lowest - <strong>Hosting/neutral/04</strong></td><td>background.default</td><td>#0F0D13</td></tr><tr><td>container lowest - <strong>Hosting/neutral/04</strong></td><td>background.paper</td><td>#0F0D13</td></tr><tr><td>secondary - <strong>Hosting/secondary/80</strong></td><td>action.hover</td><td>alpha(#C3C4E4, 0.05)</td></tr><tr><td> outline - <strong>Hosting/neutral variant/60</strong></td><td>action.disabled</td><td>alpha(#91909A, 0.6)</td></tr><tr><td>surface container highest - <strong>Hosting/neutral/22</strong></td><td>action.disabledBackground</td><td>alpha(#36343B 0.9)</td></tr></tbody></table>
