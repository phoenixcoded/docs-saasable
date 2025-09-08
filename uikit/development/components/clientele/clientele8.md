---
description: >-
  The Clientele8 component displays a centered heading and caption followed by a
  responsive, animated carousel of client logos.
---

# Clientele8



{% hint style="info" %}
All available props for the Clientele8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the clientele section.
{% endhint %}

**Component path**: `src/blocks/clientele/Clientele8.tsx`

**Component usage path:**  `src/app/blocks/clientele/clientele8/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/clientele/clientele8](https://www.saasable.io/blocks/clientele/clientele8)

## Props Details

| Prop          | Type                   | Description                                                                | Displayed as                                      |
| ------------- | ---------------------- | -------------------------------------------------------------------------- | ------------------------------------------------- |
| heading       | `string`               | The main title displayed at the top of the section.                        | `"Our Trusted Clients"`                           |
| caption       | `string`               | A brief descriptive text displayed below the heading.                      | `"We’ve worked with industry leaders worldwide."` |
| clienteleList | `ClienteleListProps[]` | An array of objects representing client logos, each containing an `image`. | `[ { image: '/logos/client1.svg' }, ... ]`        |
