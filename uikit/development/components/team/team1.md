---
description: >-
  The Team1 component displays a section with a title and caption, followed by a
  responsive grid of profile cards for team members.
---

# Team1

{% hint style="info" %}
All available props for the Team1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team1.tsx`

**Component usage path:**  `src/app/blocks/team/team1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team1**](https://www.saasable.io/blocks/team/team1)

## Props Details

| Prop        | Type                | Description                                                          | Displayed as                                                             |
| ----------- | ------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| **heading** | `string`            | Main title of the team section.                                      | `"Our Amazing Team"`                                                     |
| **caption** | `string` (Optional) | Additional context or subtitle under the heading.                    | `"Meet the talented individuals who drive our success."`                 |
| **members** | `ProfileProps[]`    | Contains data for each team member to be displayed in profile cards. | `[{ name: "John Doe", role: "CEO", avatar: "path/to/avatar.jpg" }, ...]` |
