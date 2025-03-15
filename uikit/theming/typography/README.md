---
icon: text-size
---

# Typography

SaasAble supports different typograhy for each theme, which defined in the theme's typography. You can find these in the `typography.ts` file located in specific view folders. For instance, the AI theme typography are defined in `src/views/landings/ai/theme/`.



{% tabs %}
{% tab title="src/views/landings/ai/theme/typography.ts" %}
````typescript
...

/***************************  SAAS ABLE / AI THEME - TYPOGRAPHY  ***************************/

export default function typography(theme: Theme) {
  return {
    fontFamily: FONT_ARCHIVO,

    // heading - large
    h1: {
      fontWeight: 400,
      fontSize: 57,

      // lineHeight = lineHeight in figma / fontSize. i.e 1.123 = 64/57
      lineHeight: 1.123,
      letterSpacing: -0.25,
      [theme.breakpoints.down('md')]: {
        fontSize: 45,
        lineHeight: 1.156
      },
      [theme.breakpoints.down('sm')]: {
        fontSize: 32,
        lineHeight: 1.222
      }
    },

    // heading - medium
    h2: {
      ...
    },

    // display - medium
    h3: {
      ...
    },

    // display - small
    h4: {
     ...
    },

    // label - large
    h5: {
      ...
    },

    // paragraph - large
    h6: {
      ...
    },

    // paragraph - medium
    body1: {
      ...
    },

    // paragraph - small
    body2: {
      ...
    },

    // label - medium
    subtitle1: {
      ...
    },

    // label - small
    subtitle2: {
      ...
    },

    // hyperlink - small
    caption: {
      ...
    },

    // hyperlink - large
    caption1: {
      ...
    },

    // hyperlink - medium
    caption2: {
      ...
    },

    // button
    button: {
      textTransform: 'capitalize'
    }
  };
}

```
````
{% endtab %}
{% endtabs %}

Update all values according to your requirements. for more information check[ typography page](https://www.saasable.io/sections/typography)

The more detailed info on each prop you can find from below table.

<table><thead><tr><th width="200">Typography Variant</th><th width="134">Property</th><th width="162">Value</th><th>Description</th></tr></thead><tbody><tr><td></td><td>fontFamily</td><td>FONT_ARCHIVO</td><td>It's value add from config file</td></tr><tr><td>h1 - heading - large</td><td>fontSize</td><td>57</td><td>For main heading size change</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td>For heading weight change (sets how thick or thin characters in text should be displayed)</td></tr><tr><td></td><td>lineHeight</td><td>1.123</td><td>For text height change (It sets the differences between two lines of your content)</td></tr><tr><td></td><td>letterSpacing</td><td>-0.25</td><td>For character spacing change (control the spacing between text characters)</td></tr><tr><td>h2 - heading - medium</td><td>fontSize</td><td>45</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.156</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>h3 - disaply - medium</td><td>fontSize</td><td>28</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.286</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>h4 - disaply - small</td><td>fontSize</td><td>24</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.333</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>h5 - label - large</td><td>fontSize</td><td>22</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.273</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>h6 - paragraph - large</td><td>fontSize</td><td>22</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.364</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>body1 - paragraph - medium</td><td>fontSize</td><td>16</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.5</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.5</td><td></td></tr><tr><td>body2 - paragraph - small</td><td>fontSize</td><td>14</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.429</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.25</td><td></td></tr><tr><td>subtitle1 - label - medium</td><td>fontSize</td><td>16</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.5</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.15</td><td></td></tr><tr><td>subtitle2 - label - small</td><td>fontSize</td><td>14</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>600</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.429</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.1</td><td></td></tr><tr><td>caption - hyperlink - small</td><td>fontSize</td><td>12</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>600</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.333</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0</td><td></td></tr><tr><td>caption1 - hyperlink - large</td><td>fontSize</td><td>16</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>400</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.5</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.5</td><td></td></tr><tr><td>caption2 - hyperlink - medium</td><td>fontSize</td><td>14</td><td>Same as above description</td></tr><tr><td></td><td>fontWeight</td><td>500</td><td></td></tr><tr><td></td><td>lineHeight</td><td>1.429</td><td></td></tr><tr><td></td><td>letterSpacing</td><td>0.1</td><td></td></tr></tbody></table>
