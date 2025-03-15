---
description: >-
  The Cookie1 component displays a customizable cookie consent message with a
  heading, content, and two buttons, styled within a responsive card.
---

# Cookie1

{% hint style="info" %}
All available props for the Cookie1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cookie section.
{% endhint %}

**Component path**: `src/blocks/cookie/Cookie1.tsx`

**Component usage path:**  `src/app/blocks/cookie/cookie1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cookie/cookie1**](https://www.saasable.io/blocks/cookie/cookie1)

## Props Details

| Prop             | Type                                     | Description                                                                                   | Displayed as                                                                                                                   |
| ---------------- | ---------------------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                                 | The main title of the cookie notification card.                                               | `"We use cookies to enhance your experience"`                                                                                  |
| **primaryBtn**   | `ButtonProps`                            | Properties for the primary button, typically used for the main action like accepting cookies. | `{ variant: 'contained', color: 'primary', onClick: () => console.log('Primary button clicked'), children: 'Accept' }`         |
| **secondaryBtn** | `ButtonProps`                            | Properties for the secondary button, often used for additional actions like learning more.    | `{ variant: 'outlined', color: 'secondary', onClick: () => console.log('Secondary button clicked'), children: 'Learn More' }`  |
| **cookie**       | `{ caption: string; link?: LinkProps; }` | Contains caption text and optional link for more details about cookies.                       | `{ caption: "This site uses cookies to improve your experience.", link: { href: "/privacy-policy", children: "Learn more" } }` |
