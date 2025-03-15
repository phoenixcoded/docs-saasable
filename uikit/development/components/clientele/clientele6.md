---
description: >-
  The Clientele6 component displays an optional title and a grid of client logos
  styled as Chip components, all within a responsive layout.
---

# Clientele6

{% hint style="info" %}
All available props for the Clientele6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele6.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele6/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele6](https://www.saasable.io/blocks/clientele/clientele6)

## Props Details

| Prop              | Type                   | Description                                          | Displayed as                                                                                                        |
| ----------------- | ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **title**         | `string`               | Optional heading to display above the grid of logos. | "Our Partners"                                                                                                      |
| **clienteleList** | `ClienteleListProps[]` | Array of objects with details for each client logo.  | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" }, ... ]` |
