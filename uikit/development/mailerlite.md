# MailerLite

You can use MailerLite for your email setup. SaasAble already has a working example on the "coming soon" page, which you can also utilize. You need to provide your key values in the .env file.

### Setup:

1. Mailer lite account setup
   1. Please create Mailer lite account: [https://accounts.mailerlite.com/](https://accounts.mailerlite.com/)
   2.  Integrate API: [https://dashboard.mailerlite.com/integrations/api](https://dashboard.mailerlite.com/integrations/api)

       You need to get all three things from here

       1. API Token
       2. API URL&#x20;
       3. Group ID

       <figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
You must create a new API key and Group if those do not exist.
{% endhint %}

2. Set the values from your Mailer lite account to .env file:

{% code title=".env" %}
```
##Mailerlite
MAILERLITE_API_KEY=
MAILERLITE_API_ENDPOINT=
## Use commas to separate multiple groups (Notify all groups)
MAILERLITE_GROUP=
```
{% endcode %}

3. We have already set API to send mail in the coming soon page:

{% code title="src/blocks/ComingSoon.tsx" %}
```typescript
...
 const notifMeClick = async (e: any) => {
    e.preventDefault();

    try {
      const response = await axios.post('/api/subscribe', { email });
      ...
    } catch (error) {
      ...
    }
  };
...
```
{% endcode %}

