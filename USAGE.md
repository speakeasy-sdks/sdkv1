<!-- Start SDK Example Usage -->
```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

(async () => {
    const sdk = new Jsonplaceholdertest();

    const res = await sdk.posts.getPosts();

    if (res.statusCode == 200) {
        // handle response
    }
})();

```
<!-- End SDK Example Usage -->