# Env Variables

Use a prefix `NEXT_PUBLIC_`

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title=".env" %}
```properties
## Version
VITE_APP_VERSION=v1.3.0

## Public URL
VITE_APP_BASE_URL= /
VITE_APP_API_HOST=

## Supabase
VITE_APP_SUPABASE_URL=
VITE_APP_SUPABASE_ANON_KEY=

# AWS
VITE_APP_AWS_USER_POOL_ID=
VITE_APP_AWS_USER_POOL_WEB_CLIENT_ID=
VITE_APP_AWS_REGION=

## Notify
VITE_APP_CLARITY_ID=
VITE_APP_NOTIFY_ID=
VITE_APP_ANALYTICS_ID=
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title=".env" %}
```properties
## Version
VITE_APP_VERSION=v1.3.0

## Public URL
VITE_APP_BASE_URL= /
VITE_APP_API_HOST=

## Supabase
VITE_APP_SUPABASE_URL=
VITE_APP_SUPABASE_ANON_KEY=

# AWS
VITE_APP_AWS_USER_POOL_ID=
VITE_APP_AWS_USER_POOL_WEB_CLIENT_ID=
VITE_APP_AWS_REGION=

## Notify
VITE_APP_CLARITY_ID=
VITE_APP_NOTIFY_ID=
VITE_APP_ANALYTICS_ID=
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title=".env" %}
```properties
## Version
NEXT_PUBLIC_VERSION=v1.3.0

## Public URL
NEXT_PUBLIC_PATH=
NEXT_PUBLIC_BASE_NAME=
NEXT_PUBLIC_API_HOST=

## Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

# AWS
NEXT_PUBLIC_AWS_USER_POOL_ID=
NEXT_PUBLIC_AWS_USER_POOL_WEB_CLIENT_ID=
NEXT_PUBLIC_AWS_REGION=
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title=".env" %}
```properties
## Version
NEXT_PUBLIC_VERSION=v1.3.0

## Public URL
NEXT_PUBLIC_PATH=
NEXT_PUBLIC_BASE_NAME=
NEXT_PUBLIC_API_HOST=

## Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

# AWS
NEXT_PUBLIC_AWS_USER_POOL_ID=
NEXT_PUBLIC_AWS_USER_POOL_WEB_CLIENT_ID=
NEXT_PUBLIC_AWS_REGION=
```
{% endcode %}
{% endtab %}
{% endtabs %}

For more, check here: [https://nextjs.org/docs/api-reference/next.config.js/environment-variables](https://nextjs.org/docs/api-reference/next.config.js/environment-variables)&#x20;
