---
description: >-
  The Process8 component displays a centered heading with an image and a list of
  process steps, each containing an icon, title, and description.
---

# Process8

{% hint style="info" %}
All available props for the Process8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process8.tsx`

**Component usage path:**  `src/app/blocks/process/process8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process8**](https://www.saasable.io/blocks/process/process8)

## Props Details

<table><thead><tr><th width="139">Prop</th><th width="166">Type</th><th width="174">Description</th><th>Displayed as</th></tr></thead><tbody><tr><td><strong>heading</strong></td><td><code>string</code></td><td>The main title or heading displayed at the top of the section.</td><td><code>&#x3C;Typography variant="h2/h3/h4"></code> via <code>Typeset</code> component</td></tr><tr><td><strong>caption</strong></td><td><code>string</code></td><td>A subheading or description below the heading.</td><td><code>&#x3C;Typography variant="body1"></code>inside <code>Typeset</code></td></tr><tr><td><strong>image</strong></td><td><code>ImageCommonProps</code></td><td>An object defining the image to show beside the card list.</td><td><code>&#x3C;GraphicsImage /></code> with height and responsive styles</td></tr><tr><td><strong>cards</strong></td><td><code>ProcessCardProps[]</code></td><td>Array of objects, each containing <code>icon</code>, <code>title</code>, and <code>description</code>.</td><td>Rendered inside <code>&#x3C;ListItem></code> — each item includes an avatar and text</td></tr></tbody></table>
