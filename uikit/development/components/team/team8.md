---
description: >-
  The Team8, renders a styled team member carousel with headings, captions, and
  member details using MUI, react-slick, and custom components.
---

# Team8

{% hint style="info" %}
All available props for the Team8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team8.tsx`

**Component usage path:**  `src/app/blocks/team/team8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team8**](https://www.saasable.io/blocks/team/team8)

## Props Details

| Prop        | Type                | Description                                                            | Displayed as                                                                                                         |
| ----------- | ------------------- | ---------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | Main title for the team section                                        | `"Meet Our Experts"`                                                                                                 |
| **caption** | `string` (Optional) | Subtitle or additional context for the team section                    | `"The talented individuals who make our vision a reality"`                                                           |
| **members** | `ProfileProps[]`    | List of team members, each with avatar, name, role, and optional badge | `[ { avatar: "/images/member1.jpg", name: "Alice Johnson", role: "Project Manager", badge: "Top Performer" }, ... ]` |
