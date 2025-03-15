---
description: >-
  The Process6 component displays a grid of cards, each featuring a rounded
  avatar, title, description, and a list of items with icons, all within a
  responsive layout.
---

# Process6

{% hint style="info" %}
All available props for the Process6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process6.tsx`

**Component usage path:**  `src/app/blocks/process/process6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process6**](https://www.saasable.io/blocks/process/process6)

## Props Details

| Prop        | Type                  | Description                                                        | Displayed as                                                                        |
| ----------- | --------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| **heading** | `string`              | Main heading of the section.                                       | `"Our Process Steps"`                                                               |
| **caption** | `string`              | Subheading or additional context.                                  | `"Here’s a detailed overview of each step in our process."`                         |
| **cards**   | `ProcessCardProps3[]` | Array of card objects, each containing details for a process card. | `[{ number: "01", title: "Step One", description: "Initial step...", list: [...]}]` |
