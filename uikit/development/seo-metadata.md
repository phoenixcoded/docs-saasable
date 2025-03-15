# SEO - Metadata

SaasAble maintains all static meta tags in a single place. You can refer to `src/metadata.json` for more.

All common metadata has been added to the root layout of the theme and will be rendered on all pages unless overridden at the page level.

{% tabs %}
{% tab title="src/metadata.ts" %}
```typescript
// @project
import branding from '@/branding.json';
...

/***************************  SEO METADATA - MAIN LAYOUT  ***************************/

const title = `${branding.brandName} ${branding.title}`;
const description = `${branding.brandName} is a cutting-edge software solution designed to revolutionize the way businesses operate. Our platform offers a comprehensive suite of features that enable businesses to streamline their operations, enhance productivity, and drive growth. With ${branding.brandName}, businesses can easily manage their customers, track sales, optimize marketing campaigns, and streamline their internal processes. Whether you're a startup or a large enterprise, ${branding.brandName} has the tools and expertise to help you succeed in today's fast-paced business landscape. Join the ${branding.brandName} community and experience the power of innovative software solutions for business success`;

const ogCommonMetadata = {
  locale: 'en_US',
  type: 'website',
  siteName: `${branding.brandName}`,
  images: '/assets/images/metadata/og.png' // recommended dimensions of 1200x630
};

export const mainMetadata = {
  title: {
    template: `%s | ${title}`,
    default: title // a default is required when creating a template
  },
  description,
  applicationName: title,
  keywords: [
    'SaaS',
    `${branding.brandName}`,
    'Software as a Service',
    'Cloud-based software',
    'Project management tools',
    'Enterprise software'
  ],
  creator: `${branding.company.name}`,
  metadataBase: new URL(process.env.NEXT_PUBLIC_METADATA_BASE || 'http://localhost:3000'),
  alternates: {
    canonical: '/'
  },
  openGraph: {
    title,
    description,
    url: '/',
    ...ogCommonMetadata
  }
};
```
{% endtab %}

{% tab title="branding.json" %}
```json
{
  "brandName": "SaasAble",
  "title": "React Multipurpose UI Kit and Dashboard Template",
  "company": {
    "name": "Phoenixcoded",
    "url": "https://phoenixcoded.net",
    "socialLink": {
      "linkedin": "https://in.linkedin.com/company/phoenixcoded",
      "instagram": "#",
      "facebook": "https://www.facebook.com/Phoenixcoded/",
      "youtube": "https://www.youtube.com/@Phoenixcoded",
      "github": "https://github.com/phoenixcoded",
      "dribble": "https://dribbble.com/Phoenixcoded",
      "discord": "https://discord.com/invite/AfJqqYeG",
      "support": "https://support.phoenixcoded.net"
    }
  },
  "logo": {
    "main": "",
    "logoIcon": "",
    "logoFab": "",
    "logoWatermark": ""
  }
}
```
{% endtab %}
{% endtabs %}

This JSON object later referred to a specific page for rendering. E.g. check the About page below. Any update can be made directly to `metadata.json` to affect the actual page.

{% tabs %}
{% tab title="src/metadata.ts" %}
```typescript
export const SEO_CONTENT = {
  about: {
    title: 'About',
    description: 'About'
  },

  benefit: {
    title: 'Benifit',
    description: 'Benifit'
  },
...
...
}
```
{% endtab %}

{% tab title="src/app/sections/about/page.tsx" %}
```typescript
// @next
import { Metadata } from 'next';
import dynamic from 'next/dynamic';

// @project
import { PAGE_PATH } from '@/routes/Path';
import { SEO_CONTENT } from '@/utils/constant';

const About = dynamic(() => import('@/views/sections/About'));

/***************************  METADATA - ABOUT  ***************************/

export const metadata: Metadata = { ...SEO_CONTENT.about, openGraph: { ...SEO_CONTENT.about, url: PAGE_PATH.about } };

/***************************  PAGE - ABOUT  ***************************/

export default function AboutPage() {
  return <About />;
}

```
{% endtab %}
{% endtabs %}
