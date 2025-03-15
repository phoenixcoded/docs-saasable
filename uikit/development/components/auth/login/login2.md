---
description: >-
  The Login2 component renders a responsive login page with a heading, optional
  caption, and background image, featuring social and email login options, and a
  sign-up link.
---

# Login2

{% hint style="info" %}
All available props for the Login2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Login  section.
{% endhint %}

**Component path**: `src/blocks/auth/Login/2.tsx`

**Component usage path:**  `src/app/blocks/auth/login/2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/auth/login/2](https://www.saasable.io/blocks/auth/login/2)

## Props Details

| Prop        | Type                | Description                                                                  | Displayed as                                                                        |
| ----------- | ------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| **heading** | `string`            | Main heading for the login section.                                          | "Welcome Back!"                                                                     |
| **caption** | `string` (optional) | Additional text or subtitle below the heading.                               | "Please log in to continue."                                                        |
| **image**   | `ImageCommonProps`  | Object containing image properties such as source, alt text, and dimensions. | `{ src: '/images/login-bg.jpg', alt: 'Login background', width: 500, height: 600 }` |
