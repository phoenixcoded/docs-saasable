---
description: >-
  The Clientele7 component displays an optional title, an optional button for
  navigation or actions, and a grid of client logos, all within a responsive
  layout.
---

# Clientele7

{% hint style="info" %}
All available props for the Clientele7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele7.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele7/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele7](https://www.saasable.io/blocks/clientele/clientele7)

## Props Details

| Prop              | Type                     | Description                                                    | Displayed as                                                                                                        |
| ----------------- | ------------------------ | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **title**         | `string` (optional)      | Optional heading to display at the top of the component.       | `"Our Clients"`                                                                                                     |
| **clienteleList** | `ClienteleListProps[]`   | Array of objects with details for each client logo.            | `[ { "src": "/images/client1.png", "alt": "Client 1" }, { "src": "/images/client2.png", "alt": "Client 2" }, ... ]` |
| **exploreBtn**    | `ButtonProps` (optional) | Optional button configuration, including href and other props. | `{ "variant": "outlined", "color": "primary", "href": "/explore", "children": "Explore" }`                          |
