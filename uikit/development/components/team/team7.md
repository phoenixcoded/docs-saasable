---
description: >-
  The Team7 component renders a responsive team member section with styled cards
  that reveal member details on hover.
---

# Team7

{% hint style="info" %}
All available props for the Team7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team7.tsx`

**Component usage path:**  `src/app/blocks/team/team7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team7**](https://www.saasable.io/blocks/team/team7)

## Props Details

| Prop        | Type                | Description                                                        | Displayed as                                                                                      |
| ----------- | ------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | The main title for the team section                                | `"Meet Our Team"`                                                                                 |
| **caption** | `string` (Optional) | The subtitle or description under the heading                      | `"The talented individuals who make it all happen"`                                               |
| **members** | `ProfileProps[]`    | List of team members with details including avatar, name, and role | `[ { avatar: "/images/team/member1.jpg", name: "Alice Johnson", role: "Project Manager" }, ... ]` |
