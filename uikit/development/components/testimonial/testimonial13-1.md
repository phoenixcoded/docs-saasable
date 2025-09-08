---
description: >-
  A responsive testimonial slider component built with MUI, Framer Motion, and
  react-slick, showcasing user reviews with avatars and roles.
---

# Testimonial13

{% hint style="info" %}
All available props for the Testimonial13 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial13.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial13/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial13**](https://www.saasable.io/blocks/testimonial/testimonial13)

## Props Details

<table><thead><tr><th width="149">Prop</th><th>Type</th><th>Description</th><th>Displayed as</th></tr></thead><tbody><tr><td>heading</td><td><code>object</code></td><td>Heading data (title, subtitle, alignment etc.) passed to the Typeset component</td><td><code>{ title: "Our Happy Clients", subtitle: "What people say about us" }</code></td></tr><tr><td>primaryBtn</td><td><code>object</code>(optional)</td><td>Optional button props to show a CTA next to the heading</td><td><code>{ children: "Join Us", href: "/signup" }</code></td></tr><tr><td>testimonials</td><td><code>array of objects</code></td><td>List of testimonial items containing user profile and review</td><td><code>[{ profile: { name, role, avatar }, review }]</code></td></tr></tbody></table>

