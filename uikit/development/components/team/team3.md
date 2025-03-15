# Team3

The `Team3` component presents a team section with animated transitions, featuring a heading, caption, and a responsive slider displaying team members. Each card includes an image with an overlay, member details, and social media links, with dots navigation at the bottom.

{% hint style="info" %}
All available props for the Team3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team3.tsx`

**Component usage path:**  `src/app/blocks/team/team3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team3**](https://www.saasable.io/blocks/team/team3)

## Props Details

| Prop        | Type                | Description                                                                                                                   | Display as                                                                                                           |
| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | The main heading/title for the section.                                                                                       | `"Our Leadership Team"`                                                                                              |
| **caption** | `string` (Optional) | A subtitle or brief description of the team.                                                                                  | `"Meet the people driving our success."`                                                                             |
| **members** | `ProfileProps[]`    | An array of objects representing the team members. Each contains properties like `name`, `role`, `avatar`, and `socialLinks`. | `[ { name: "Alice", role: "CEO", avatar: "/images/alice.jpg", socialLinks: { linkedin: "url", instagram: "url" } }]` |
