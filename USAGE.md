<!-- Start SDK Example Usage -->


```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";
import { DeletePostsIdResponse } from "jsonplaceholdertest/dist/sdk/models/operations";

const sdk = new Jsonplaceholdertest();

sdk.post.deletePostsId({
  id: "<ID>",
}).then((res: DeletePostsIdResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```
<!-- End SDK Example Usage -->