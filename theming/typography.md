# Typography

Applying a single configuration across all relevant components. You can find these in the `typography.ts` file located in the specific src folders. For instance, single typography is defined in `src/themes/`.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/themes/typography.ts" %}
```typescript

// @project
import { ThemeFonts } from '@/config';

/***************************  DEFAULT - TYPOGRAPHY  ***************************/

export default function typography() {
  return {
    fontFamily: ThemeFonts.FONT_ARCHIVO,
    letterSpacing: 0,

    // heading - h1
    h1: {
      fontWeight: 500,
      fontSize: 40,
      lineHeight: '44px'
    },

    // heading - h2
    h2: {
      ...
    },

    // heading - h3
    h3: {
      ...
    },

    // heading - h4
    h4: {
      ...
    },

    // heading - h5
    h5: {
      ...
    },

    // heading - h6
    h6: {
      ...
    },

    // subtitle - 1
    subtitle1: {
      ...
    },

    // subtitle - 2
    subtitle2: {
      ...
    },

    // paragraph - 1
    body1: {
      ...
    },

    // paragraph - 2
    body2: {
      ...
    },

    // caption - regular
    caption: {
      ...
    },

    // caption - medium
    caption1: {
      ...
    },

    // button
    button: {
      textTransform: 'capitalize'
    }
  };
}
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/themes/typography.js" %}
```javascript

// @project
import { ThemeFonts } from '@/config';

/***************************  DEFAULT - TYPOGRAPHY  ***************************/

export default function typography() {
  return {
    fontFamily: ThemeFonts.FONT_ARCHIVO,
    letterSpacing: 0,

    // heading - h1
    h1: {
      fontWeight: 500,
      fontSize: 40,
      lineHeight: '44px'
    },

    // heading - h2
    h2: {
      ...
    },

    // heading - h3
    h3: {
      ...
    },

    // heading - h4
    h4: {
      ...
    },

    // heading - h5
    h5: {
      ...
    },

    // heading - h6
    h6: {
      ...
    },

    // subtitle - 1
    subtitle1: {
      ...
    },

    // subtitle - 2
    subtitle2: {
      ...
    },

    // paragraph - 1
    body1: {
      ...
    },

    // paragraph - 2
    body2: {
      ...
    },

    // caption - regular
    caption: {
      ...
    },

    // caption - medium
    caption1: {
      ...
    },

    // button
    button: {
      textTransform: 'capitalize'
    }
  };
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/themes/typography.ts" %}
```typescript

// @project
import { FONT_ARCHIVO } from '@/config';

/***************************  DEFAULT - TYPOGRAPHY  ***************************/

export default function typography() {
  return {
    fontFamily: FONT_ARCHIVO,
    letterSpacing: 0,

    // heading - h1
    h1: {
      fontWeight: 500,
      fontSize: 40,
      lineHeight: '44px'
    },

    // heading - h2
    h2: {
      ...
    },

    // heading - h3
    h3: {
      ...
    },

    // heading - h4
    h4: {
      ...
    },

    // heading - h5
    h5: {
      ...
    },

    // heading - h6
    h6: {
      ...
    },

    // subtitle - 1
    subtitle1: {
      ...
    },

    // subtitle - 2
    subtitle2: {
      ...
    },

    // paragraph - 1
    body1: {
      ...
    },

    // paragraph - 2
    body2: {
      ...
    },

    // caption - regular
    caption: {
      ...
    },

    // caption - medium
    caption1: {
      ...
    },

    // button
    button: {
      textTransform: 'capitalize'
    }
  };
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/themes/typography.js" %}
```typescript

// @project
import { FONT_ARCHIVO } from '@/config';

/***************************  DEFAULT - TYPOGRAPHY  ***************************/

export default function typography() {
  return {
    fontFamily: FONT_ARCHIVO,
    letterSpacing: 0,

    // heading - h1
    h1: {
      fontWeight: 500,
      fontSize: 40,
      lineHeight: '44px'
    },

    // heading - h2
    h2: {
      ...
    },

    // heading - h3
    h3: {
      ...
    },

    // heading - h4
    h4: {
      ...
    },

    // heading - h5
    h5: {
      ...
    },

    // heading - h6
    h6: {
      ...
    },

    // subtitle - 1
    subtitle1: {
      ...
    },

    // subtitle - 2
    subtitle2: {
      ...
    },

    // paragraph - 1
    body1: {
      ...
    },

    // paragraph - 2
    body2: {
      ...
    },

    // caption - regular
    caption: {
      ...
    },

    // caption - medium
    caption1: {
      ...
    },

    // button
    button: {
      textTransform: 'capitalize'
    }
  };
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

Update all values according to your requirements. For more information, check the [typography page](https://admin.saasable.io/data-display/typography)

The more detailed info on each prop can be found in the table below.

<table><thead><tr><th width="200">Typography Variant</th><th width="134">Property</th><th width="162">Value</th><th>Description</th></tr></thead><tbody><tr><td></td><td>fontFamily</td><td>FONT_ARCHIVO</td><td>It's value add from config file</td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td>For character spacing change (control the spacing between text characters)</td></tr><tr><td>h1 - heading</td><td>fontSize</td><td>40</td><td>For main heading size change</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td>For heading weight change (sets how thick or thin characters in text should be displayed)</td></tr><tr><td></td><td>lineHeight</td><td>'44px'</td><td>For text height change (It sets the differences between two lines of your content)</td></tr><tr><td>h2 - heading</td><td>fontSize</td><td>32</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'36px'</td><td></td></tr><tr><td>h3 - heading</td><td>fontSize</td><td>28</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'32px'</td><td></td></tr><tr><td>h4 - heading</td><td>fontSize</td><td>24</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'28px'</td><td></td></tr><tr><td>h5 - heading</td><td>fontSize</td><td>20</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'24px'</td><td></td></tr><tr><td>h6 - heading</td><td>fontSize</td><td>18</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'22px'</td><td></td></tr><tr><td>subtitle1 - subtitle - 1</td><td>fontSize</td><td>16</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'20px'</td><td></td></tr><tr><td>subtitle2 - subtitle - 2</td><td>fontSize</td><td>14</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'18px'</td><td></td></tr><tr><td>body1 - paragraph - 1</td><td>fontSize</td><td>16</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'20px'</td><td></td></tr><tr><td>body2 - paragraph - 2</td><td>fontSize</td><td>14</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'18px'</td><td></td></tr><tr><td>caption - caption - regular</td><td>fontSize</td><td>12</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'16px'</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>caption1 - caption - medium</td><td>fontSize</td><td>12</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>'16px'</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr></tbody></table>
