---
description: >-
  We have implemented custom SVG icons along with Tabler fill and stroke icons
  using the SVGSprite method.
---

# Icon

Each method for adding SVG icons varies slightly. You can explore all available icons on our [icon page](https://www.saasable.io/sections/icon)&#x20;

You can manage all icons in one place using a common component, `SvgIcon.tsx` , located in the `components` folder.

## Props Details

<table><thead><tr><th width="178.33333333333331">Prop</th><th width="215">Type</th><th>Description</th></tr></thead><tbody><tr><td><strong>name</strong></td><td><code>string</code></td><td>Keep always Svg ID value = name of icon value</td></tr><tr><td><strong>size</strong></td><td><code>number</code> (optional)</td><td>Adjusts the size of the SVG icon. The default size is set to 24</td></tr><tr><td><strong>type</strong></td><td><code>IconType</code></td><td>Currently, the default value is <code>IconType.STROKE</code> set for the tabler outline icon. Another type is <code>IconType.FILL</code> for tabler fill icon  &#x26; <code>IconType.CUSTOM</code> for custom icon svg adding</td></tr><tr><td><strong>color</strong></td><td><code>string</code> (optional)</td><td>To change color of the svg icon</td></tr><tr><td><strong>stroke</strong></td><td><code>number</code> (optional)</td><td>Adjusts the stroke width of the SVG icon. This prop is <strong>not applied</strong> when the icon type is <code>IconType.FILL</code>.</td></tr><tr><td><strong>twoToneColor</strong></td><td><code>string</code> (optional)</td><td>To change seondary color of the svg icon which is <strong>only used</strong> in <code>IconType.CUSTOM</code> icon type or twotone icon</td></tr></tbody></table>

<details>

<summary>How to use Icons dynamically?</summary>

Icons can be set dynamically based on conditions in SaasAble. you need to pass the type as Custom (`IconType.CUSTOM`). Check the following code snippet where it is being used:

**Note**: your name should already exist here for the dynamic icon: _public/assets/svg/sprite-custom.svg_

```typescript
// @project
import { IconType } from '@/enum';

export const feature6 = {
  // other data...
  features: [
    {
      icon: { name: 'custom-data', type: IconType.CUSTOM }, // Icon data
      title: 'Bring your Data Model',
      content: 'Collect relevant customer information efficiently.'
    },
    ...
  ]
};
```

</details>
