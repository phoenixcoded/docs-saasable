---
description: >-
  The Cookie3 component displays a cookie notification with a customizable
  heading, message, and buttons, styled within a responsive graphics card
  layout.
---

# Cookie3

{% hint style="info" %}
All available props for the Cookie3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cookie section.
{% endhint %}

**Component path**: `src/blocks/cookie/Cookie3.tsx`

**Component usage path:**  `src/app/blocks/cookie/cookie3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cookie/cookie3**](https://www.saasable.io/blocks/cookie/cookie3)

## Props Details

| Prop             | Type                                     | Description                                                                                   | Displayed as                                                                                                                      |
| ---------------- | ---------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                                 | Main title of the cookie notification card.                                                   | `"Special Offer Just for You"`                                                                                                    |
| **cookie**       | `{ caption: string; link?: LinkProps; }` | Contains caption text and an optional link for more details about cookies.                    | `{ caption: "We use cookies to ensure you get the best experience.", link: { href: "/privacy-policy", children: "Learn more" } }` |
| **primaryBtn**   | `ButtonProps`                            | Properties for the primary button, typically used for the main action like accepting cookies. | `{ variant: 'outlined', color: 'primary', onClick: () => console.log('Primary button clicked'), children: 'Accept' }`             |
| **secondaryBtn** | `ButtonProps`                            | Properties for the secondary button, often used for additional actions or information.        | `{ variant: 'contained', color: 'secondary', onClick: () => console.log('Secondary button clicked'), children: 'Learn More' }`    |
