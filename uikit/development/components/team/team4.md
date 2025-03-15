# Team4

The `Team4` component displays a team section with a centered heading, caption, and a slider featuring team members' cards. Each card includes a background image, optional badge, and member details, with responsive settings for different screen sizes.

{% hint style="info" %}
All available props for the Team4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team4.tsx`

**Component usage path:**  `src/app/blocks/team/team4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team4**](https://www.saasable.io/blocks/team/team4)

## Props Details

<table><thead><tr><th>Prop</th><th width="207">Type</th><th>Description</th><th>Displayed as</th></tr></thead><tbody><tr><td><strong>heading</strong></td><td><code>string</code></td><td>Main title of the section.</td><td><code>"Our Amazing Team"</code></td></tr><tr><td><strong>caption</strong></td><td><code>string</code> (Optional)</td><td>Additional context or subtitle.</td><td><code>"Meet the talented individuals driving our success."</code></td></tr><tr><td><strong>members</strong></td><td><code>ProfileProps[]</code></td><td>Contains data for each team member to be displayed in cards.</td><td><code>[{ name: 'Henrietta Bayer', role: 'Chief Technology Officer', avatar: '/assets/images/profile/profile-2.png', badge: 'Best Employee of the year' }, ...]</code></td></tr></tbody></table>
