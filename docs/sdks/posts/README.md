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
import { GetPostsResponse } from "jsonplaceholdertest/dist/sdk/models/operations";

const sdk = new Jsonplaceholdertest();

sdk.posts.getPosts().then((res: GetPostsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.GetPostsResponse](../../models/operations/getpostsresponse.md)>**


## postPosts

Create a new post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";
import { PostPostsResponse } from "jsonplaceholdertest/dist/sdk/models/operations";

const sdk = new Jsonplaceholdertest();

sdk.posts.postPosts({
  body: "Operative haptic",
  id: 7574.44,
  title: "Stage brightly morph",
  userId: 175.83,
}).then((res: PostPostsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `request`                                                    | [shared.Post](../../models/shared/post.md)                   | :heavy_check_mark:                                           | The request object to use for the request.                   |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.PostPostsResponse](../../models/operations/postpostsresponse.md)>**

