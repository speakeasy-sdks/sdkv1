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

(async() => {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.deletePostsId({
    id: "<ID>",
  });

  if (res.statusCode == 200) {
    // handle response
  }
})();
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

(async() => {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.getPostsId({
    id: "<ID>",
  });

  if (res.statusCode == 200) {
    // handle response
  }
})();
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

(async() => {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.putPostsId({
    id: "<ID>",
    post: {},
  });

  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                                    | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `request`                                                                    | [operations.PutPostsIdRequest](../../models/operations/putpostsidrequest.md) | :heavy_check_mark:                                                           | The request object to use for the request.                                   |
| `config`                                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                 | :heavy_minus_sign:                                                           | Available config options for making requests.                                |


### Response

**Promise<[operations.PutPostsIdResponse](../../models/operations/putpostsidresponse.md)>**

