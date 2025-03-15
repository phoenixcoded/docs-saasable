# Color

SaasAble supports different colors for each theme, with colors defined in the theme's palette. You can find these in the `palette.ts` file located in specific view folders. For instance, the AI theme colors are defined in `src/views/landings/ai/theme/`.



{% tabs %}
{% tab title="src/views/landings/ai/theme/palette.ts" %}
```typescript

/***************************  DEFAULT/AI THEME - PALETTE  ***************************/

export default function palette(mode: ThemeMode) {
  ... 
  ...
  const lightPalette = {
    primary: {
      lighter: '#CCE5FF', // AI/primary/90 - primary container / primary fixed
      light: '#92CCFF', // AI/primary/80 - primary fixed dim
      main: '#006397', // AI/primary/40 - primary
      dark: '#004B73', // AI/primary/30 - on primary fixed variant
      darker: '#001D31' // AI/primary/10 - on primary container / on primary fixed
    },
    ...
  };

  const darkPalette = {
    primary: {
      lighter: '#004B73', // AI/primary/30 - primary container / on primary fixed variant
      light: '#3398DB', // AI/primary/60 - primary fixed dim
      main: '#92CCFF', // AI/primary/80 - primary
      dark: '#CCE5FF ', // AI/primary/90 - on primary container / primary fixed
      darker: '#E7F2FF' // AI/primary/95 - on primary container / on primary fixed
    },
    ...
  };
  ...
}

```
{% endtab %}
{% endtabs %}



The details below contain the default theme which is **AI theme**. for more information check [color page](https://www.saasable.io/sections/color)

### Light mode color

#### 🎨 Primary color&#x20;

<table><thead><tr><th width="356">Name</th><th width="222">Variable name</th><th width="166">Color</th></tr></thead><tbody><tr><td>primary - <strong>AI/primary/40</strong></td><td>primary.main</td><td> #006397</td></tr><tr><td>primary container / primary fixed - <strong>AI/primary/90</strong></td><td>primary.lighter</td><td>#CCE5FF </td></tr><tr><td>primary fixed dim - <strong>AI/primary/80</strong></td><td>primary.light</td><td>#92CCFF </td></tr><tr><td>on primary fixed variant - <strong>AI/primary/30</strong></td><td>primary.dark</td><td>#004B73</td></tr><tr><td>on primary container / on primary fixed - <strong>AI/primary/10</strong></td><td>primary.darker</td><td>#001D31</td></tr></tbody></table>

#### 🎨 Secondary color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>secondary - <strong>AI/secondary/40</strong></td><td>secondary.main</td><td>#4F6070 </td></tr><tr><td>secondary container / secondary fixed - <strong>AI/secondary/90</strong></td><td>secondary.lighter</td><td>#D3E4F8</td></tr><tr><td>secondary fixed dim - <strong>AI/secondary/80</strong></td><td>secondary.light</td><td>#B7C8DB</td></tr><tr><td>on secondary fixed variant - <strong>AI/secondary/30</strong></td><td>secondary.dark</td><td>#384858</td></tr><tr><td>on secondary container / on primary fixed - <strong>AI/secondary/10</strong></td><td>secondary.darker</td><td>#0B1D2B</td></tr></tbody></table>

#### 🎨 Neutral

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface / surface bright - <strong>AI/neutral/98</strong></td><td>grey.50</td><td>#F9F9FC</td></tr><tr><td>surface container low - <strong>AI/neutral/96</strong></td><td>grey.100</td><td>#F1F4F9</td></tr><tr><td>surface container - <strong>AI/neutral/94</strong></td><td>grey.200</td><td>#EBEEF3</td></tr><tr><td>surface container high - <strong>AI/neutral/92</strong></td><td>grey.300</td><td>#E6E8EE</td></tr><tr><td>surface container highest - <strong>AI/neutral/90</strong></td><td>grey.400</td><td>#E2E2E5</td></tr><tr><td>surface dim - <strong>AI/neutral/87</strong></td><td>grey.500</td><td>#D7DADF</td></tr><tr><td>outline variant - <strong>AI/neutral variant/80</strong> (divider)</td><td>grey.600</td><td>#C2C7CE</td></tr><tr><td>outline - <strong>AI/neutral variant/50</strong></td><td>grey.700</td><td>#72787E</td></tr><tr><td>on surface variant - <strong>AI/neutral variant/30</strong>  (textSecondary)</td><td>grey.800</td><td>#42474E</td></tr><tr><td>on surface - <strong>AI/neutral/10</strong> (textPrimary)</td><td>grey.900</td><td>#1A1C1E</td></tr></tbody></table>

### Dark mode color

#### 🎨 Primary color&#x20;

<table><thead><tr><th width="356">Name</th><th width="222">Variable name</th><th width="166">Color</th></tr></thead><tbody><tr><td>primary - <strong>AI/primary/80</strong></td><td>primary.main</td><td>#92CCFF</td></tr><tr><td>primary container / on primary fixed variant - <strong>AI/primary/30</strong></td><td>primary.lighter</td><td>#004B73</td></tr><tr><td>primary fixed dim - <strong>AI/primary/60</strong></td><td>primary.light</td><td>#3398DB</td></tr><tr><td>on primary container / primary fixed - <strong>AI/primary/90</strong></td><td>primary.dark</td><td>#CCE5FF</td></tr><tr><td>on primary container / on primary fixed - <strong>AI/primary/95</strong></td><td>primary.darker</td><td>#E7F2FF</td></tr></tbody></table>

#### 🎨 Secondary color

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>secondary - <strong>AI/secondary/80</strong></td><td>secondary.main</td><td>#B7C8DB</td></tr><tr><td>secondary container / on secondary fixed variant - <strong>AI/secondary/30</strong></td><td>secondary.lighter</td><td>#384858</td></tr><tr><td>secondary fixed dim - <strong>AI/secondary/60</strong></td><td>secondary.light</td><td>#8193A4</td></tr><tr><td>on secondary container / secondary fixed - <strong>AI/secondary/90</strong></td><td>secondary.dark</td><td>#D3E4F8</td></tr><tr><td>on secondary container / on primary fixed - <strong>AI/secondary/95</strong></td><td>secondary.darker</td><td>#E7F2FF</td></tr></tbody></table>

#### 🎨 Neutral

<table><thead><tr><th width="360.3333333333333">Name</th><th width="229">Variable name</th><th>Color</th></tr></thead><tbody><tr><td>surface / surface dim - <strong>AI/neutral/06</strong></td><td>grey.50</td><td>#101418</td></tr><tr><td>surface container low - <strong>AI/neutral/10</strong></td><td>grey.100</td><td>#1A1C1E</td></tr><tr><td>surface container - <strong>AI/neutral/12</strong></td><td>grey.200</td><td>#1C2024</td></tr><tr><td>surface container high - <strong>AI/neutral/17</strong></td><td>grey.300</td><td>#272A2E</td></tr><tr><td>surface container highest - <strong>AI/neutral/22</strong></td><td>grey.400</td><td>#313539</td></tr><tr><td>surface container lowest - <strong>AI/neutral/04</strong> (backgroundDark)</td><td>grey.500</td><td>#0B0F12</td></tr><tr><td>outline variant - <strong>AI/neutral variant/30</strong> (dividerDark)</td><td>grey.600</td><td>#42474E</td></tr><tr><td>outline - <strong>AI/neutral variant/60</strong></td><td>grey.700</td><td>#8C9198</td></tr><tr><td>on surface variant - <strong>AI/neutral variant/80</strong>  (textSecondaryDark)</td><td>grey.800</td><td>#C2C7CE</td></tr><tr><td>on surface - <strong>AI/neutral/90</strong> (textPrimaryDark)</td><td>grey.900</td><td>#E2E2E5</td></tr></tbody></table>
