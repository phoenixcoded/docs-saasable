# Guest Guard

A **Guest Guard** restricts access to certain pages for authenticated users, redirecting them away from areas like login or signup if they’re already logged in. Ideal for enhancing user flow and preventing redundant actions.\
\
**Guest guard** is configured at **`src/utils/route-guard/GuestGuard.tsx`**\
\
We have used it the same as follows:

```typescript
<GuestGuard>
      <AuthLayout>{children}</AuthLayout>
</GuestGuard>
```
