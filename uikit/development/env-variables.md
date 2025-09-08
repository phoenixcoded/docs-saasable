# Env Variables

Use a prefix `NEXT_PUBLIC_`

{% code title=".env" %}
```typescript
## Version
NEXT_PUBLIC_VERSION=v1.3.0

## Public URL
NEXT_PUBLIC_PATH=
NEXT_PUBLIC_BASE_NAME=

## SEO
NEXT_PUBLIC_METADATA_BASE=https://www.saasable.io

NEXT_PUBLIC_CLARITY_ID=

## Notify
NEXT_PUBLIC_NOTIFY_ID=

## Google Analytics
NEXT_PUBLIC_ANALYTICS_ID=

## Mailerlite
MAILERLITE_API_KEY=
MAILERLITE_API_ENDPOINT=https://connect.mailerlite.com/api
## Use commas to separate multiple groups (Notify all groups)
MAILERLITE_GROUP=
```
{% endcode %}

For more, check here: [https://nextjs.org/docs/api-reference/next.config.js/environment-variables](https://nextjs.org/docs/api-reference/next.config.js/environment-variables)&#x20;
