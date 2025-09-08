# Hero18

The `Hero18` component is a **visually-rich hero section** used in landing pages. It combines **a call-to-action**, **headline text**, and **decorative image lists** to create an engaging introduction section.



{% hint style="info" %}
All available props for the Hero18 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero18.tsx`

**Component usage path:**  `src/app/blocks/hero/hero18/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero18**](https://www.saasable.io/blocks/hero/hero18)

## Props Details

| Prop            | Type                                                          | Description                                      | Displayed as                                                     |
| --------------- | ------------------------------------------------------------- | ------------------------------------------------ | ---------------------------------------------------------------- |
| headLine        | <p><code>string</code> or</p><p><code>ReactElement</code></p> | Main headline text.                              | `"Welcome to Our Next Big Thing"`                                |
| **captionLine** | <p><code>string</code> or</p><p><code>ReactElement</code></p> | Subtitle or short description below the headline | `"Smaller text below the heading"`                               |
| imageList       | `{ image: string \| ImageComponentProps }[]`                  | List of images to showcase visually              | `"Row of logos/images at the bottom"`                            |
| exploreBtn      | `ButtonProps`                                                 | Optional properties for an "Explore" button.     | `{ children: "Explore Now", href: "/explore", variant: "outline` |

