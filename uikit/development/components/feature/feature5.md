---
description: >-
  The Feature5 component creates a responsive, multi-section feature display
  with images, feature cards, avatar groups, and optional action buttons.
---

# Feature5

{% hint style="info" %}
All available props for the Feature5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature5.tsx`

**Component usage path:**  `src/app/blocks/feature/feature5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature5**](https://www.saasable.io/blocks/feature/feature5)

## Props Details

| Prop              | Type                                                              | Description                                        | Displayed as                                                                                                                            |
| ----------------- | ----------------------------------------------------------------- | -------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**       | `string`                                                          | Main title of the feature section.                 | `"Our New Features"`                                                                                                                    |
| **caption**       | `string`                                                          | Subtitle or additional description.                | `"Discover the latest updates and features"`                                                                                            |
| **image1**        | `ImageCommonProps`                                                | Primary image for the section.                     | <p><code>"path-to-image1.svg"</code><br> or <br><code>{ light: 'path-to-image1-light.svg', dark: 'path-to-image1-dark.svg' }</code></p> |
| **image2**        | `ImageCommonProps` (Optional)                                     | Secondary image for the section.                   | <p><code>"path-to-image2.svg"</code><br> or <br><code>{ light: 'path-to-image2-light.svg', dark: 'path-to-image2-dark.svg' }</code></p> |
| **features**      | `IconCardProps[]`                                                 | Array of feature objects for the first section.    | `[ { icon: 'icon-name-1', title: 'Feature 1', content: 'Description of feature 1' }, ... ]`                                             |
| **features2**     | `IconCardProps[]` (Optional)                                      | Additional feature objects for the second section. | `[ { icon: 'icon-name-3', title: 'Feature 3', content: 'Description of feature 3' } ]`                                                  |
| **profileGroups** | `{ avatarGroups: AvatarGroupProps[]; review: string }` (Optional) | Contains avatars and review text.                  | `{ avatarGroups: [ { avatar: 'path-to-avatar1.jpg' }, ... ], review: 'What our users say about us' }`                                   |
| **content**       | `string` (Optional)                                               | Additional content for the second section.         | `"Learn more about our advanced features and benefits"`                                                                                 |
| **actionBtn**     | `ButtonProps` (Optional)                                          | Properties for the primary action button.          | `{ variant: 'contained', color: 'primary', onClick: () => { alert('Button Clicked!'); }, children: 'Learn More' }`                      |
| **actionBtn2**    | `ButtonProps` (Optional)                                          | Properties for the secondary action button.        | `{ variant: 'outlined', color: 'secondary', onClick: () => { alert('Button 2 Clicked!'); }, children: 'See All Features' }`             |
| isCoverImage1     | `boolean`                                                         | Affects `image1` styling                           | If `true`, image stretches and covers background.                                                                                       |
| features          | `IconCardProps[]`                                                 | First section right below heading                  | Displays list of features using `IconCard`.                                                                                             |
| isCoverImage2     | boolean                                                           | If `true`, image stretches and covers background.  | Affects `image2` styling                                                                                                                |

