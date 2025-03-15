# Auth Guard

An **Auth Guard** protects specific pages by ensuring only authenticated users can access them.

Auth Guard is configured at **`src/utils/route-guard/AuthGuard.tsx`**\
\
To use it just wrap component with **AuthGuard**, same as below.

```typescript
<AuthProvider>
    <AuthGuard>
        ...
        <YourReactComponent />
        ...
    </AuthGuard>
</AuthProvider>
```
