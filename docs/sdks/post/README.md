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

async function run() {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.deletePostsId({
    id: "<ID>",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                              | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `request`                                                                              | [operations.DeletePostsIdRequest](../../sdk/models/operations/deletepostsidrequest.md) | :heavy_check_mark:                                                                     | The request object to use for the request.                                             |
| `config`                                                                               | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                           | :heavy_minus_sign:                                                                     | Available config options for making requests.                                          |


### Response

**Promise<[operations.DeletePostsIdResponse](../../sdk/models/operations/deletepostsidresponse.md)>**
### Errors

| Error Object                     | Status Code                      | Content Type                     |
| -------------------------------- | -------------------------------- | -------------------------------- |
| errors.DeletePostsIdResponseBody | 404                              | application/json                 |
| errors.SDKError                  | 4xx-5xx                          | */*                              |

## getPostsId

Get a single post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.getPostsId({
    id: "<ID>",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                        | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `request`                                                                        | [operations.GetPostsIdRequest](../../sdk/models/operations/getpostsidrequest.md) | :heavy_check_mark:                                                               | The request object to use for the request.                                       |
| `config`                                                                         | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                     | :heavy_minus_sign:                                                               | Available config options for making requests.                                    |


### Response

**Promise<[operations.GetPostsIdResponse](../../sdk/models/operations/getpostsidresponse.md)>**
### Errors

| Error Object                  | Status Code                   | Content Type                  |
| ----------------------------- | ----------------------------- | ----------------------------- |
| errors.GetPostsIdResponseBody | 404                           | application/json              |
| errors.SDKError               | 4xx-5xx                       | */*                           |

## putPostsId

Update a post

### Example Usage

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
  const sdk = new Jsonplaceholdertest();

  const res = await sdk.post.putPostsId({
    id: "<ID>",
    post: {},
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                        | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `request`                                                                        | [operations.PutPostsIdRequest](../../sdk/models/operations/putpostsidrequest.md) | :heavy_check_mark:                                                               | The request object to use for the request.                                       |
| `config`                                                                         | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                     | :heavy_minus_sign:                                                               | Available config options for making requests.                                    |


### Response

**Promise<[operations.PutPostsIdResponse](../../sdk/models/operations/putpostsidresponse.md)>**
### Errors

| Error Object                  | Status Code                   | Content Type                  |
| ----------------------------- | ----------------------------- | ----------------------------- |
| errors.PutPostsIdResponseBody | 404                           | application/json              |
| errors.SDKError               | 4xx-5xx                       | */*                           |
