---
description: This docs cover how can you add or update fant family for specific theme
---

# Font Family

1. Import new package for font family (Ignore if you want to use existing and provided font family with saasable). To add free Google fonts refer [google fonts](https://fonts.google.com/)
2. Update the config to consider new font family and export it.

{% tabs %}
{% tab title="src/config.ts" %}
```typescript
// @next
import { Archivo, Figtree, Roboto } from 'next/font/google'; // Add new font family

// Create variable for font family
const fontRobot = Roboto({ subsets: ['latin'], weight: ['100', '300', '400', '500', '700', '900'] });

// Export the new font family
export const FONT_ROBOTO: string = fontRobot.style.fontFamily;
```
{% endtab %}
{% endtabs %}

3. Update the typography to apply to the chosen theme.&#x20;

{% tabs %}
{% tab title="src/views/landings/ai/theme/typography.ts" %}
<pre class="language-typescript"><code class="lang-typescript">import { Theme } from '@mui/material/styles';

// @project
import { FONT_ROBOTO } from '@/config'; // refer new font family

export default function typography(theme: Theme) {
  return {
<strong>    fontFamily: FONT_ROBOTO, // change font
</strong>    // other settings
  };
}
</code></pre>
{% endtab %}
{% endtabs %}
