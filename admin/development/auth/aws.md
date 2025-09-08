# AWS

1.  **Set AWS Config**

    Currently, AWS uses a dummy config, so we don't need to change anything, but in actual implementation, you need to set poolId and appClientId in the following file. For more details, refer to AWS here: [https://aws.amazon.com/cognito/](https://aws.amazon.com/cognito/)
2. Change the **auth provider** in the **config** file.

{% code title="src/config.ts" %}
```typescript
...
export const AUTH_PROVIDER: AuthType = AuthType.AWS;
...
```
{% endcode %}

2. Add your **AwsUserpoolID,** webClientId, and aws region in the **.env** file.

{% code title=".env" %}
```properties
...

# AWS
NEXT_PUBLIC_AWS_USER_POOL_ID=
NEXT_PUBLIC_AWS_USER_POOL_WEB_CLIENT_ID=
NEXT_PUBLIC_AWS_REGION=
```
{% endcode %}



🎉 **Congrats!** Supabase is now configured in your project. 🚀 You can test it by running the project.
