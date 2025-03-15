---
description: >-
  This is a static footer component. Simply import it wherever you need to use
  it in your project.
---

# Footer

We offer 7 different variants of footer designs to suit various styles and requirements. You can explore all available footer options by visiting the [footer page](https://www.saasable.io/sections/footer). Here’s an example of how to import a footer component:

<pre class="language-svg" data-title="layout.tsx"><code class="lang-svg">// @project
<strong>import { Footer3 } from '@/blocks/footer'; // Import footer variant here
</strong>import ThemeCustomization from './theme';

// @types
import { ChildrenProps } from '@/types/root';

/***************************  LAYOUT - AI  ***************************/

export default function AILayout({ children }: ChildrenProps) {
  return (
    &#x3C;ThemeCustomization>
      &#x3C;>
        {/* other section */}

        {/* footer section */}
<strong>        &#x3C;Footer3 /> // Use import footer variant
</strong>      &#x3C;/>
    &#x3C;/ThemeCustomization>
  );
}
</code></pre>

