# jsonplaceholdertest

<div align="left">
    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
    <a href="https://github.com/speakeasy-sdks/sdkv1.git/actions"><img src="https://img.shields.io/github/actions/workflow/status/speakeasy-sdks/sdkv1/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
    
</div>

<!-- Start SDK Installation [installation] -->
## SDK Installation

### NPM

```bash
npm add jsonplaceholdertest
```

### Yarn

```bash
yarn add jsonplaceholdertest
```
<!-- End SDK Installation [installation] -->

<!-- Start SDK Example Usage [usage] -->
## SDK Example Usage

### Example

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

<!-- Start Available Resources and Operations [operations] -->
## Available Resources and Operations

### [posts](docs/sdks/posts/README.md)

* [getPosts](docs/sdks/posts/README.md#getposts) - Returns all posts
* [postPosts](docs/sdks/posts/README.md#postposts) - Create a new post

### [post](docs/sdks/post/README.md)

* [deletePostsId](docs/sdks/post/README.md#deletepostsid) - Delete a post
* [getPostsId](docs/sdks/post/README.md#getpostsid) - Get a single post
* [putPostsId](docs/sdks/post/README.md#putpostsid) - Update a post
<!-- End Available Resources and Operations [operations] -->



<!-- Start Error Handling [errors] -->
## Error Handling

Handling errors in this SDK should largely match your expectations.  All operations return a response object or throw an error.  If Error objects are specified in your OpenAPI Spec, the SDK will throw the appropriate Error type.

| Error Object                     | Status Code                      | Content Type                     |
| -------------------------------- | -------------------------------- | -------------------------------- |
| errors.DeletePostsIdResponseBody | 404                              | application/json                 |
| errors.SDKError                  | 4xx-5xx                          | */*                              |

Example

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
    const sdk = new Jsonplaceholdertest();

    let res;
    try {
        res = await sdk.post.deletePostsId({
            id: "<id>",
        });
    } catch (err) {
        if (err instanceof errors.DeletePostsIdResponseBody) {
            console.error(err); // handle exception
            throw err;
        } else if (err instanceof errors.SDKError) {
            console.error(err); // handle exception
            throw err;
        }
    }

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End Error Handling [errors] -->



<!-- Start Server Selection [server] -->
## Server Selection

### Select Server by Index

You can override the default server globally by passing a server index to the `serverIdx: number` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:

| # | Server | Variables |
| - | ------ | --------- |
| 0 | `https://jsonplaceholder.typicode.com` | None |

#### Example

```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
    const sdk = new Jsonplaceholdertest({
        serverIdx: 0,
    });

    const res = await sdk.posts.getPosts();

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```


### Override Server URL Per-Client

The default server can also be overridden globally by passing a URL to the `serverURL: str` optional parameter when initializing the SDK client instance. For example:
```typescript
import { Jsonplaceholdertest } from "jsonplaceholdertest";

async function run() {
    const sdk = new Jsonplaceholdertest({
        serverURL: "https://jsonplaceholder.typicode.com",
    });

    const res = await sdk.posts.getPosts();

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End Server Selection [server] -->



<!-- Start Custom HTTP Client [http-client] -->
## Custom HTTP Client

The Typescript SDK makes API calls using the [axios](https://axios-http.com/docs/intro) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `AxiosInstance` object.

For example, you could specify a header for every request that your sdk makes as follows:

```typescript
import { jsonplaceholdertest } from "Jsonplaceholdertest";
import axios from "axios";

const httpClient = axios.create({
    headers: {'x-custom-header': 'someValue'}
})

const sdk = new Jsonplaceholdertest({defaultClient: httpClient});
```
<!-- End Custom HTTP Client [http-client] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
