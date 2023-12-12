<!-- Start SDK Example Usage [usage] -->
```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
    const sdk = new Jsonplaceholdertest();

    const res = await sdk.posts.getPosts();

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End SDK Example Usage [usage] -->