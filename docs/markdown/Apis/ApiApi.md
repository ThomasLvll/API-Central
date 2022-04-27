# ApiApi

All URIs are relative to *http://141.94.79.199:2001*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSlugDelete**](ApiApi.md#apiSlugDelete) | **DELETE** /api/{slug} | 
[**apiSlugGet**](ApiApi.md#apiSlugGet) | **GET** /api/{slug} | 
[**apiSlugHead**](ApiApi.md#apiSlugHead) | **HEAD** /api/{slug} | 
[**apiSlugOptions**](ApiApi.md#apiSlugOptions) | **OPTIONS** /api/{slug} | 
[**apiSlugPatch**](ApiApi.md#apiSlugPatch) | **PATCH** /api/{slug} | 
[**apiSlugPost**](ApiApi.md#apiSlugPost) | **POST** /api/{slug} | 
[**apiSlugPut**](ApiApi.md#apiSlugPut) | **PUT** /api/{slug} | 
[**apiSlugTrace**](ApiApi.md#apiSlugTrace) | **TRACE** /api/{slug} | 
[**apisGet**](ApiApi.md#apisGet) | **GET** /apis | 
[**apisIdGet**](ApiApi.md#apisIdGet) | **GET** /apis/{id} | 
[**apisIdPatch**](ApiApi.md#apisIdPatch) | **PATCH** /apis/{id} | 
[**apisPost**](ApiApi.md#apisPost) | **POST** /apis | 


<a name="apiSlugDelete"></a>
# **apiSlugDelete**
> apiSlugDelete(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugGet"></a>
# **apiSlugGet**
> apiSlugGet(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugHead"></a>
# **apiSlugHead**
> apiSlugHead(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugOptions"></a>
# **apiSlugOptions**
> apiSlugOptions(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugPatch"></a>
# **apiSlugPatch**
> apiSlugPatch(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugPost"></a>
# **apiSlugPost**
> apiSlugPost(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugPut"></a>
# **apiSlugPut**
> apiSlugPut(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apiSlugTrace"></a>
# **apiSlugTrace**
> apiSlugTrace(slug)



    Calls an API by slug.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**| URL slug of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apisGet"></a>
# **apisGet**
> List apisGet()



    Gets a list of available served APIs. API only shows up if user has the \\&#39;index\\&#39; permission on its context.

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/API.md)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apisIdGet"></a>
# **apisIdGet**
> API apisIdGet(id)



    Gets an API by ID. User must have the \\&#39;view-api\\&#39; permission on its context.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of API. | [default to null]

### Return type

[**API**](../Models/API.md)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apisIdPatch"></a>
# **apisIdPatch**
> apisIdPatch(id)



    Updates an API by ID. User must have the \\&#39;modify-api\\&#39; permission on its context.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of API. | [default to null]

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="apisPost"></a>
# **apisPost**
> ResourceCreated apisPost(API)



    Creates an API. User must have the \\&#39;create-api\\&#39; permission on \\&#39;central\\&#39; context.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **API** | [**API**](../Models/API.md)| API to create. | [optional]

### Return type

[**ResourceCreated**](../Models/ResourceCreated.md)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/plain

