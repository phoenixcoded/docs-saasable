---
description: >-
  The Process1 component displays a section with an accordion-style card list
  and an optional side image, incorporating animations and dynamic content based
  on the provided props.
---

# Process1

{% hint style="info" %}
All available props for the Process1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process1.tsx`

**Component usage path:**  `src/app/blocks/process/process1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process1**](https://www.saasable.io/blocks/process/process1)

## Props Details

<table><thead><tr><th width="179">Prop </th><th>Type</th><th>Description</th><th>Displayed as</th></tr></thead><tbody><tr><td><strong>heading</strong></td><td><code>string</code></td><td>Main title for the component.</td><td><code>"Streamlined Workflow"</code></td></tr><tr><td><strong>caption</strong></td><td><code>string</code></td><td>Additional text under the heading.</td><td><code>"An overview of our efficient process to enhance productivity."</code></td></tr><tr><td><strong>image</strong></td><td><code>ImageCommonProps</code></td><td>Image path or object with <code>light</code> and <code>dark</code> image path.</td><td><code>"path-to-image.svg"</code><br>or<br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></td></tr><tr><td><strong>cards</strong></td><td><code>ProcessCardProps[]</code></td><td>Array of cards with details to display.</td><td><code>[ { title: "Initial Setup", description: "Setting up...", list: [...], icon: "setup-icon" }, ... ]</code></td></tr><tr><td><strong>defaultExpanded</strong></td><td><code>string</code> (Optional)</td><td>Default expanded panel ID.</td><td>Pass panelId to open it default.</td></tr></tbody></table>
