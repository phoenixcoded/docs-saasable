---
description: >-
  A responsive blog detail page built with MUI, displaying an article with
  author info, social icons, a featured image, and a breakdown of the five
  stages of design thinking.
---

# BlogDetails

The `BlogDetails` component presents a detailed, engaging blog post focused on the **Design Thinking process**. It combines visual storytelling with structured content to enhance user engagement and readability. This component is built using **Material-UI (MUI)** and leverages responsive design principles for seamless performance across devices.

{% code title="blogDetails.tsx" %}
```svg
// @project
import BlogDetail from '@/blocks/BlogDetails';
import ContainerWrapper from '@/components/ContainerWrapper';

/***************************  SECTIONS - BLOG DETAILS  ***************************/

export default function BlogDetails() {
  return (
    <>
      {/* other setion  */}

      {/* Blog Details   */}

      <ContainerWrapper>
        <BlogDetail />
      </ContainerWrapper>
    </>
  );
}

```
{% endcode %}

