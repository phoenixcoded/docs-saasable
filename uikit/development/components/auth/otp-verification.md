---
description: >-
  The OTP Verification component renders an OTP verification page with a title,
  a caption showing an email address, an OTP input form, and a "Resend Code"
  link, styled with background elements .
---

# OTP Verification

{% hint style="info" %}
All available props for the OtpVerification component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the OtpVerification section.
{% endhint %}

**Component path**: `src/blocks/auth/OtpVerification.tsx`

**Component usage path:**  `src/app/blocks/auth/otp-verification/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/auth/otp-verification](https://www.saasable.io/blocks/auth/otp-verification)

## Props Details

| Prop Name	  | Type                              | Description                                           | Displayed as                                                     |
| ----------- | --------------------------------- | ----------------------------------------------------- | ---------------------------------------------------------------- |
| **heading** | `string`                          | Main title or heading for the OTP verification page.  | `"Enter the OTP"`                                                |
| **caption** | `{ text: string; email: string }` | Object containing the caption text and email address. | `{ text: "A code has been sent to", email: "user@example.com" }` |
