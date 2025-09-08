# AWS

1.  **Set AWS Config**

    Currently, AWS uses a dummy config, so we don't need to change anything, but in actual implementation, you need to set poolId and appClientId in the following file. For more details, refer to AWS here: [https://aws.amazon.com/cognito/](https://aws.amazon.com/cognito/)
2. Change the **auth provider** in the **config** file.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/config.ts" %}
```typescript
...
export const AUTH_PROVIDER: AuthType = AuthType.AWS;
...
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/config.js" %}
```javascript
...
export const AUTH_PROVIDER = AuthType.AWS;
...
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/config.ts" %}
```properties
...
export const AUTH_PROVIDER: AuthType = AuthType.AWS;
...
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/config.js" %}
```javascript
...
export const AUTH_PROVIDER = AuthType.AWS;
...
```
{% endcode %}
{% endtab %}
{% endtabs %}

2. Add your **AwsUserpoolID,** webClientId, and aws region in the **.env** file.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title=".env" %}
```properties
...

# AWS
VITE_APP_AWS_USER_POOL_ID=
VITE_APP_AWS_USER_POOL_WEB_CLIENT_ID=
VITE_APP_AWS_REGION=
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-properties" data-title=".env"><code class="lang-properties"><strong>...
</strong><strong>
</strong><strong># AWS
</strong>VITE_APP_AWS_USER_POOL_ID=
VITE_APP_AWS_USER_POOL_WEB_CLIENT_ID=
VITE_APP_AWS_REGION=
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title=".env" %}
```properties
...

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
...

# AWS
NEXT_PUBLIC_AWS_USER_POOL_ID=
NEXT_PUBLIC_AWS_USER_POOL_WEB_CLIENT_ID=
NEXT_PUBLIC_AWS_REGION=
```
{% endcode %}
{% endtab %}
{% endtabs %}



🎉 **Congrats!** Supabase is now configured in your project. 🚀 You can test it by running the project.
