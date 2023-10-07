# jsonplaceholdertest

<div align="left">
    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
    <a href="https://github.com/speakeasy-sdks/sdkv1.git/actions"><img src="https://img.shields.io/github/actions/workflow/status/speakeasy-sdks/sdkv1/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
    
</div>

<!-- Start SDK Installation -->
## SDK Installation

### NPM

```bash
npm add jsonplaceholdertest
```

### Yarn

```bash
yarn add jsonplaceholdertest
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->
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
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations


### [post](docs/sdks/post/README.md)

* [deletePostsId](docs/sdks/post/README.md#deletepostsid) - Delete a post
* [getPostsId](docs/sdks/post/README.md#getpostsid) - Get a single post
* [putPostsId](docs/sdks/post/README.md#putpostsid) - Update a post

### [posts](docs/sdks/posts/README.md)

* [getPosts](docs/sdks/posts/README.md#getposts) - Returns all posts
* [postPosts](docs/sdks/posts/README.md#postposts) - Create a new post
<!-- End SDK Available Operations -->

<!-- Start Dev Containers -->

<!-- End Dev Containers -->

<!-- Start Pagination -->
# Pagination

Some of the endpoints in this SDK support pagination. To use pagination, you make your SDK calls as usual, but the
returned response object will have a `next` method that can be called to pull down the next group of results. If the
return value of `next` is `null`, then there are no more pages to be fetched.

Here's an example of one such pagination call:
<!-- End Pagination -->

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
