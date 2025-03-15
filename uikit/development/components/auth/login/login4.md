---
description: >-
  The Login4 component renders a login page with user reviews, a main heading,
  counters for additional details, and authentication forms with social login
  options.
---

# Login4

{% hint style="info" %}
All available props for the Login4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Login  section.
{% endhint %}

**Component path**: `src/blocks/auth/Login/4.tsx`

**Component usage path:**  `src/app/blocks/auth/login/4/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/auth/login/4](https://www.saasable.io/blocks/auth/login/4)

## Props Details

| Prop Name       | Type                                                              | Description                                                       | Displayed as                                                                 |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **reviewData**  | `{ avatarList: string[]; rating: number; totalReviews: string; }` | User review details including avatars, rating, and total reviews. | `{ avatarList: ['url1', 'url2'], rating: 4.5, totalReviews: '123 reviews' }` |
| **heading**     | `string`                                                          | Main title or heading for the page.                               | `"Welcome to Our Service"`                                                   |
| **blockDetail** | `BlockProps[]`                                                    | Array of objects with details for counter blocks.                 | `[{ counter: '100', caption: 'Users', defaultUnit: '+' }]`                   |
