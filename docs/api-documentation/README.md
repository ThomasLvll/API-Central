<!-- PROJECT HEADER -->
<div align="center">
  <!-- <img src="docs/img/logo.png" alt="Logo" width="80" height="80">
  --><h3 align="center"><a href="https://github.com/ThomasLvll/API-Central">API Central</a> › <a href="../">Documentation</a> › API</h3>
</div>



<a name="documentation-for-api-endpoints"></a>
## API Endpoints

All URIs are relative to *http://141.94.79.199:2001*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ApiApi* | [**apiSlugDelete**](Apis/ApiApi.md#apislugdelete) | **DELETE** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugGet**](Apis/ApiApi.md#apislugget) | **GET** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugHead**](Apis/ApiApi.md#apislughead) | **HEAD** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugOptions**](Apis/ApiApi.md#apislugoptions) | **OPTIONS** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugPatch**](Apis/ApiApi.md#apislugpatch) | **PATCH** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugPost**](Apis/ApiApi.md#apislugpost) | **POST** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugPut**](Apis/ApiApi.md#apislugput) | **PUT** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apiSlugTrace**](Apis/ApiApi.md#apislugtrace) | **TRACE** /api/{slug} | Calls an API by slug.
*ApiApi* | [**apisGet**](Apis/ApiApi.md#apisget) | **GET** /apis | Gets a list of available served APIs. API only shows up if user has the \\'index\\' permission on its context.
*ApiApi* | [**apisIdGet**](Apis/ApiApi.md#apisidget) | **GET** /apis/{id} | Gets an API by ID. User must have the \\'view-api\\' permission on its context.
*ApiApi* | [**apisIdPatch**](Apis/ApiApi.md#apisidpatch) | **PATCH** /apis/{id} | Updates an API by ID. User must have the \\'modify-api\\' permission on its context.
*ApiApi* | [**apisPost**](Apis/ApiApi.md#apispost) | **POST** /apis | Creates an API. User must have the \\'create-api\\' permission on \\'central\\' context.
*AuthApi* | [**tokenGet**](Apis/AuthApi.md#tokenget) | **GET** /token | Gets an API token.
*AuthApi* | [**tokenVerifyGet**](Apis/AuthApi.md#tokenverifyget) | **GET** /token/verify | Verifies the supplied API token.
*CallExternalApi* | [**apiSlugDelete**](Apis/CallExternalApi.md#apislugdelete) | **DELETE** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugGet**](Apis/CallExternalApi.md#apislugget) | **GET** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugHead**](Apis/CallExternalApi.md#apislughead) | **HEAD** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugOptions**](Apis/CallExternalApi.md#apislugoptions) | **OPTIONS** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugPatch**](Apis/CallExternalApi.md#apislugpatch) | **PATCH** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugPost**](Apis/CallExternalApi.md#apislugpost) | **POST** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugPut**](Apis/CallExternalApi.md#apislugput) | **PUT** /api/{slug} | Calls an API by slug.
*CallExternalApi* | [**apiSlugTrace**](Apis/CallExternalApi.md#apislugtrace) | **TRACE** /api/{slug} | Calls an API by slug.
*DefaultApi* | [**statusGet**](Apis/DefaultApi.md#statusget) | **GET** /status | Gets the server status.


<a name="documentation-for-models"></a>
## Models

 - [API](./Models/API.md)
 - [APIPermission](./Models/APIPermission.md)
 - [Error](./Models/Error.md)
 - [Meta](./Models/Meta.md)
 - [ResourceCreated](./Models/ResourceCreated.md)
 - [ResourceCreated_urls](./Models/ResourceCreated_urls.md)
 - [ResourceUpdated](./Models/ResourceUpdated.md)
 - [ResourceUpdated_updatedFields](./Models/ResourceUpdated_updatedFields.md)


<a name="documentation-for-authorization"></a>
## Authorization

<a name="apiToken"></a>
### apiToken

- **Type**: HTTP basic authentication

<a name="authToken"></a>
### authToken

- **Type**: HTTP basic authentication

