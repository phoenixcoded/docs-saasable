---
description: >-
  The Clientele5 component features an optional title, a responsive slider for
  client logos, and an optional description, all within a structured layout.
---

# Clientele5

{% hint style="info" %}
All available props for the Clientele5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele5.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele5/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele5](https://www.saasable.io/blocks/clientele/clientele5)

## Props Details

| Prop              | Type                   | Description                                                    | Displayed as                                                                                                        |
| ----------------- | ---------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **title**         | `string` (Optional)    | Optional subtitle to display on the left side of the carousel. | "Our Valued Partners"                                                                                               |
| **clienteleList** | `ClienteleListProps[]` | Array of objects with details for each client logo.            | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" }, ... ]` |
| **description**   | `string` (Optional)    | Optional description to display below the carousel.            | "We proudly showcase our esteemed partners."                                                                        |
