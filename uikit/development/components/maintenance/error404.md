---
description: >-
  Error404Page that displays a full-page error 404 message with an image, a
  heading, and an optional button, all within a styled container.
---

# Error404

{% hint style="info" %}
All available props for the Error404 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the maintenance section.
{% endhint %}

**Component path**: `src/blocks/maintenance/Error404.tsx`

**Component usage path:**  `src/app/blocks/error404/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/maintenance/error404**](https://www.saasable.io/blocks/maintenance/error404)

## Props Details

| Prop           | Type          | Description                                 | Displayed as                                                                          |
| -------------- | ------------- | ------------------------------------------- | ------------------------------------------------------------------------------------- |
| **heading**    | `string`      | Main message or heading for the error page. | `"Oops! Page Not Found"`                                                              |
| **primaryBtn** | `ButtonProps` | Properties for the primary button.          | `{ variant: "contained", size: "medium", children: "Go Home", onClick: handleClick }` |
