---
description: >-
  The Clientele1 component displays a horizontally scrolling marquee of client
  logos with an optional title, adjusting for RTL language direction.
---

# Clientele1

{% hint style="info" %}
All available props for the Clientele1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele1.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele1](https://www.saasable.io/blocks/clientele/clientele1)

## Props Details

| Prop              | Type                   | Description                                 | Displayed as                              |
| ----------------- | ---------------------- | ------------------------------------------- | ----------------------------------------- |
| **title**         | `string` (Optional)    | Title or subtitle for the clientele section | `"Our Esteemed Clients"`                  |
| **clienteleList** | `ClienteleListProps[]` | List of clients or partners with image data | See the `Example Structure` section above |
