# Posts
(*posts*)

### Available Operations

* [getPosts](#getposts) - Returns all posts
* [postPosts](#postposts) - Create a new post

## getPosts

Returns all posts

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

(async() => {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.posts.getPosts();

  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.GetPostsResponse](../../sdk/models/operations/getpostsresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 400-600         | */*             |

## postPosts

Create a new post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

(async() => {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.posts.postPosts({});

  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `request`                                                    | [shared.Post](../../sdk/models/shared/post.md)               | :heavy_check_mark:                                           | The request object to use for the request.                   |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.PostPostsResponse](../../sdk/models/operations/postpostsresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 400-600         | */*             |
