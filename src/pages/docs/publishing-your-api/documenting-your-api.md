---
title: "Generating API documentation"
updated: 2023-07-21
contextual_links:
  - type: section
    name: "Additional resources"
  - type: subtitle
    name: "Videos"
  - type: link
    name: "Collaboration & Documentation | Postman Enterprise"
    url: "https://youtu.be/u1yEOo0dPfk"
  - type: link
    name: "API Publishers Series, Part 1: Introduction to Documentation"
    url: "https://youtu.be/z4egejVO20M"
  - type: link
    name: "API Publishers Series, Part 2: Increase Adoption of your Public API"
    url: "https://youtu.be/52pXP3X4a_8"
  - type: dynamic_blog
    name: "Blog posts"
    blog_tag: "documentation"
  - type: subtitle
    name: "Case Studies"
  - type: link
    name: "WhatsApp uses API documentation tools to enhance collaboration"
    url:  "https://www.postman.com/case-studies/whatsapp/"
  - type: link
    name: "SEI Novus uses documentation to keep business use cases solved"
    url: "https://www.postman.com/case-studies/sei-novus/"
---

[Documentation](https://www.postman.com/api-platform/api-documentation/) is an important part of any collection or API. Good documentation helps the people who use your collection to understand what it does and how each request works. And comprehensive API documentation lets your consumers know what endpoints are available and how to interact with them.

Once you've generated documentation for your collection or API, users can [view the documentation](/docs/publishing-your-api/viewing-documentation/) in Postman. By default your documentation is private, so you must share a collection or API with others before they can access it. If you're creating a public API, you can [publish your documentation](/docs/publishing-your-api/publishing-your-docs/) to make it publicly available to anyone with a web browser.

## Contents

* [Documenting a collection](#documenting-a-collection)
    * [Documenting gRPC and WebSocket collections](#documenting-grpc-and-websocket-collections)
* [Generating API documentation](#generating-api-documentation)
    * [Viewing schema documentation](#viewing-schema-documentation)
    * [Creating new documentation for an API](#creating-new-documentation-for-an-api)
    * [Adding existing documentation to an API](#adding-existing-documentation-to-an-api)
    * [Editing API documentation](#editing-api-documentation)
    * [Deleting API documentation](#deleting-api-documentation)
* [Associating environments with documentation](#associating-environments-with-documentation)
* [Next steps](#next-steps)

## Documenting a collection

Postman automatically generates basic documentation for any collection you create. [View the documentation](/docs/publishing-your-api/viewing-documentation/) for details about all of the requests in your collection, along with sample code in various client languages. Request details include the method, authorization type, URL, headers, request and response structures, and examples. In addition, the documentation displays all key-value pairs for request parameters, headers, and bodies.

To make your documentation even more valuable to users, [add descriptions](/docs/publishing-your-api/authoring-your-documentation/) to the items in your collection. Any descriptions you add are automatically included in the documentation for your collection.

To add a description to a collection or folder, do the following:

1. Select **Collections** in the sidebar, and then select a collection or a folder.
1. Enter a description in the **Overview** tab. To learn more about using Postman's built-in editing tools, see [Writing your docs](/docs/publishing-your-api/authoring-your-documentation/).
1. Select outside of the editor to save your new content.

<img alt="Documenting a collection" src="https://assets.postman.com/postman-docs/v10/documentation-overview-tab-v10.jpg" >

To add a description to a request, do the following:

1. Select **Collections** in the sidebar, and then select a request.
1. Select the documentation icon <img alt="Documentation icon" src="https://assets.postman.com/postman-docs/documentation-icon-v8-10.jpg#icon" width="16px"> in the right sidebar.
1. Enter a description in the right sidebar. To learn more about using Postman's built-in editing tools, see [Writing your docs](/docs/publishing-your-api/authoring-your-documentation/).
1. Select outside of the editor to save your new content.

<img alt="Documenting a request" src="https://assets.postman.com/postman-docs/v10/documentation-pane-v10.jpg" width="600px">

> You can also edit descriptions when viewing the complete documentation for a collection. Select a collection in the sidebar, then select **View complete documentation** in the **Overview** tab. From here, you can add a description to any item in the collection.

### Documenting gRPC and WebSocket collections

Collections with gRPC or WebSocket requests use a different format than collections with HTTP requests. You can view documentation and add descriptions for gRPC or WebSocket requests. You can also add a description on the collection's **Overview** tab, but you can't view or edit documentation for the full collection. Learn more about [documenting gRPC requests](/docs/sending-requests/grpc/grpc-request-interface/#the-right-sidebar) or [documenting WebSocket requests](/docs/sending-requests/websocket/websocket/#documenting-requests).

## Generating API documentation

The API Builder provides one place to view, create, and manage all of your API's documentation. Postman automatically generates API docs for any OpenAPI 2.0 or 3.0 definition. You can also add detailed documentation to any API by generating a collection from the API or by adding a copy of an existing collection.

### Viewing schema documentation

If you are [designing an API](/docs/designing-and-developing-your-api/developing-an-api/defining-an-api/) based on the OpenAPI 2.0 or 3.0 specification, Postman automatically creates documentation based on your API definition.

The API documentation includes complete API, path, and operation information, such as authentication methods, parameters, request bodies, response bodies and headers, and examples. The documentation also includes information for various data models, such as required attributes, default, minimum, and maximum values, and other constraints.

To view the documentation for an OpenAPI 2.0 or 3.0 API, do the following:

1. Select **APIs** in the sidebar and select an API.
1. On the API's overview, under **Definition**, select **View schema documentation**.

<img alt="Viewing schema documentation" src="https://assets.postman.com/postman-docs/v10/documentation-view-schema-docs-v10-16.jpg" />

### Creating new documentation for an API

To generate a new collection for API documentation, do the following:

1. Select **APIs** in the sidebar and select an API.
1. On the API's overview, next to **Collections**, select **+** and select **Generate from definition**.
1. Change any settings to customize the new collection.
1. Select **Generate Collection**.

The new collection displays on your API's overview and under your API in the sidebar. To view documentation for the collection, select the collection and select **View complete documentation**.

<img alt="Generating new API documentation" src="https://assets.postman.com/postman-docs/v10/documentation-generate-api-docs-v10-16.jpg" />

### Adding existing documentation to an API

To use an existing collection for API documentation, do the following:

1. Select **APIs** in the sidebar and select an API.
1. On the API's overview, next to **Collections**, select **+** and select **Copy existing collection**.
1. Select an available collection and select **Copy Collection**.

The copy of the collection displays on your API's overview and under your API in the sidebar. To view documentation for the collection, select the collection and select **View complete documentation**.

<img alt="Adding existing API documentation" src="https://assets.postman.com/postman-docs/v10/documentation-add-api-docs-v10-16.jpg" />

> When you add a collection, an independent copy of the collection is added to the API. The copy in the API will no longer be in sync with the original. If you move or delete an API, any collections contained in the API are moved or deleted with it.

### Editing API documentation

You can add to your API documentation collections from the API Builder.

To edit a documentation collection for an API, do the following:

1. Select **APIs** in the sidebar and select an API.
1. On the API's overview, select a collection and select **View complete documentation**.
1. Enter a description for any item. To learn more about using Postman's built-in editing tools, see [Writing your docs](/docs/publishing-your-api/authoring-your-documentation/).
1. Select outside of the editor to save your new content.

> Schema documentation can't be edited directly. Instead, [edit your API's definition](/docs/designing-and-developing-your-api/developing-an-api/defining-an-api/) and then select **Save**. Postman automatically updates the API docs to reflect the latest changes to your definition.

<img alt="Editing API documentation" src="https://assets.postman.com/postman-docs/v10/documentation-editing-api-docs-v10-16.jpg" />

### Deleting API documentation

To delete a documentation collection from an API, do the following:

1. Select **APIs** in the sidebar and select an API.
1. On the API's overview, select the more actions icon <img alt="More actions icon" src="https://assets.postman.com/postman-docs/icon-more-actions-v9.jpg#icon" width="16px"> next to a collection and select **Delete**.

## Associating environments with documentation

An [environment](/docs/sending-requests/managing-environments/) is a set of related [variables](/docs/sending-requests/variables/) you can use in Postman requests. You can also refer to variables when [writing descriptions](/docs/publishing-your-api/authoring-your-documentation/) in a collection. In each case, the initial value of the variable is automatically populated in the documentation.

Anyone using your collection will be able to view the variables in the documentation if the associated environment is also shared with them. For public documentation, you can select an environment during the [publishing process](/docs/publishing-your-api/publishing-your-docs/). Publishing an environment makes it available to anyone [viewing public documentation](/docs/publishing-your-api/viewing-documentation/).

To use an environment variable in your documentation, do the following:

1. [Create a new environment](/docs/sending-requests/managing-environments/#creating-environments) if one doesn't already exist.
1. Make the environment active by selecting it in the [environment dropdown list](/docs/sending-requests/managing-environments/#selecting-an-active-environment).
1. If needed, [add a new variable](/docs/sending-requests/managing-environments/#adding-environment-variables) to the environment.
1. Add a [reference to the variable](/docs/sending-requests/variables/#accessing-variables) to requests or descriptions in your collection.

<img alt="Referencing a variable" src="https://assets.postman.com/postman-docs/v10/documentation-add-variable-v10-16.jpg" width="566px">

> If someone imports a collection using the **Run in Postman** button from your documentation, they will also import the environment and any associated variables. The initial values for variables are published in your documentation, so make sure they don't contain any sensitive data.

## Next steps

After generating API documentation in Postman, you can edit and format the docs and publish them.

* To learn more about editing and formatting your documentation, visit [Writing your docs](/docs/publishing-your-api/authoring-your-documentation/).
* To learn how to make your documentation publicly available, visit [Publishing your docs](/docs/publishing-your-api/publishing-your-docs/).
