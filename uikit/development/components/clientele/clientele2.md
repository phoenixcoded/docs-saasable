---
description: >-
  The Clientele2 component renders a list of client logos in a flexible row
  layout, with an optional title, and features a fade-in animation.
---

# Clientele2

{% hint style="info" %}
All available props for the Clientele2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele2.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele2](https://www.saasable.io/blocks/clientele/clientele2)

## Props Details

| Prop Name         | Type                   | Description                                         | Displayed as                                                                                                   |
| ----------------- | ---------------------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **title**         | `string` (Optional)    | Optional title to display above the client logos.   | "Our Valued Clients"                                                                                           |
| **clienteleList** | `ClienteleListProps[]` | Array of objects with details for each client logo. | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" } ]` |
