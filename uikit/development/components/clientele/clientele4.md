---
description: >-
  The Clientele4 component displays an optional title and a grid of client logos
  with responsive layout and spacing.
---

# Clientele4

{% hint style="info" %}
All available props for the Clientele4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele4.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele4/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele4](https://www.saasable.io/blocks/clientele/clientele4)

## Props Details

| Prop              | Type                   | Description                                           | Displayed as                                                                                                        |
| ----------------- | ---------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **title**         | `string` (Optional)    | Optional subtitle to display above the grid of logos. | "Our Valued Partners"                                                                                               |
| **clienteleList** | `ClienteleListProps[]` | Array of objects with details for each client logo.   | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" }, ... ]` |
