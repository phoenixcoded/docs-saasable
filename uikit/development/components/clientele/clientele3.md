---
description: >-
  The Clientele3 component displays an optional title and a responsive carousel
  of client logos, styled as Chip components with a gradient overlay effect.
---

# Clientele3

{% hint style="info" %}
All available props for the Clientele3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele3.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele3/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele3](https://www.saasable.io/blocks/clientele/clientele3)

## Props Details

| Prop              | Type                   | Description	                                           | Displayed as                                                                                                        |
| ----------------- | ---------------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| **title**         | `string` (Optional)    | Optional title to display above the carousel of logos. | "Our Esteemed Clients"                                                                                              |
| **clienteleList** | `ClienteleListProps[]` | Array of objects with details for each client logo.    | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" }, ... ]` |
