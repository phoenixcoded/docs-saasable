# Feature26

**`Feature26`** displays a central captioned heading with three vertically-aligned animated feature blocks, combining icons, text content, images, and a group avatar visualization.

{% hint style="info" %}
All available props for the Feature26 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature26.tsx`

**Component usage path:**  `src/app/blocks/feature/feature26/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/feature/feature23)[**https://stage.saasable.io/blocks/feature/feature26**](https://stage.saasable.io/blocks/feature/feature26)

## Props Details

| Prop        | Type                 | Description                                                                   | Display As                                                  |
| ----------- | -------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------- |
| headLine    | `string`             | The title or heading that is displayed at the top of the section.             | Rendered at the top center via the `Typeset` component.     |
| captionLine | `string` (Optional)  | A short subheading or caption displayed below the headline.                   | Rendered below the heading in smaller font.                 |
| feature1    | `FeatureProps`       | Contains icon, title, description (content), and image for the left feature.  | Displayed with text first, then image (on left column).     |
| feature2    | `FeatureProps`       | Contains icon, title, description (content), and image for the right feature. | Displayed with image first, then text (on right column).    |
| feature3    | `{ title, content }` | The central feature’s title and description. No image/icon here.              | Displayed in the center, with avatars and watermark logo.   |
| avatarList  | `string[]`           | List of avatar image URLs shown around a central logo.                        | Shown in a circular group via the `AvatarGalaxy` component. |
