# Post
(*post*)

### Available Operations

* [deletePostsId](#deletepostsid) - Delete a post
* [getPostsId](#getpostsid) - Get a single post
* [putPostsId](#putpostsid) - Update a post

## deletePostsId

Delete a post

### Example Usage

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

### Parameters

| Parameter                                                                          | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `request`                                                                          | [operations.DeletePostsIdRequest](../../models/operations/deletepostsidrequest.md) | :heavy_check_mark:                                                                 | The request object to use for the request.                                         |
| `config`                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                       | :heavy_minus_sign:                                                                 | Available config options for making requests.                                      |


### Response

**Promise<[operations.DeletePostsIdResponse](../../models/operations/deletepostsidresponse.md)>**


## getPostsId

Get a single post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";
import { GetPostsIdResponse } from "jsonplaceholdertest/dist/sdk/models/operations";

const sdk = new Jsonplaceholdertest();

sdk.post.getPostsId({
  id: "<ID>",
}).then((res: GetPostsIdResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                    | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `request`                                                                    | [operations.GetPostsIdRequest](../../models/operations/getpostsidrequest.md) | :heavy_check_mark:                                                           | The request object to use for the request.                                   |
| `config`                                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                 | :heavy_minus_sign:                                                           | Available config options for making requests.                                |


### Response

**Promise<[operations.GetPostsIdResponse](../../models/operations/getpostsidresponse.md)>**


## putPostsId

Update a post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";
import { PutPostsIdResponse } from "jsonplaceholdertest/dist/sdk/models/operations";

const sdk = new Jsonplaceholdertest();

sdk.post.putPostsId({
  id: "<ID>",
  post: {
    body: "whoever",
    id: 9539.46,
    title: "Tennessine hacking",
    userId: 476.95,
  },
}).then((res: PutPostsIdResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                    | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `request`                                                                    | [operations.PutPostsIdRequest](../../models/operations/putpostsidrequest.md) | :heavy_check_mark:                                                           | The request object to use for the request.                                   |
| `config`                                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                 | :heavy_minus_sign:                                                           | Available config options for making requests.                                |


### Response

**Promise<[operations.PutPostsIdResponse](../../models/operations/putpostsidresponse.md)>**

