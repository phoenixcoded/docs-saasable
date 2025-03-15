# Team2

The `Team2` component displays a carousel of team members using `react-slick`. It features a slider with customizable settings, displaying each team member's profile in a `GraphicsCard` with a background image and overlay. The component adjusts the number of visible slides based on screen size and uses the `Typeset` component to show the team member's name and role. The styling adapts to both light and dark themes.

{% hint style="info" %}
All available props for the Team2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team2.tsx`

**Component usage path:**  `src/app/blocks/team/team2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team2**](https://www.saasable.io/blocks/team/team2)

## Props Details

| Prop        | Type                | Description                                                                                           | Displayed as                                                                                                            |
| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | The main heading or title of the section that introduces the team.                                    | `"Meet Our Team"`                                                                                                       |
| **caption** | `string` (Optional) | A subtitle or caption that gives a brief description of the team or the purpose of the section.       | `"Our dedicated team of experts"`                                                                                       |
| **members** | `ProfileProps[]`    | An array of team members, where each member has properties like `name`, `role`, and `avatar` (image). | `[{ name: "John Doe", role: "CEO", avatar: "path/to/avatar.jpg" }, { name: "Jane Smith", role: "CTO", avatar: "..." }]` |
