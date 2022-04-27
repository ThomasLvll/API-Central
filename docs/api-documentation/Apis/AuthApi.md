# AuthApi

All URIs are relative to *http://141.94.79.199:2001*

Method | HTTP request | Description
------------- | ------------- | -------------
[**tokenGet**](AuthApi.md#tokenGet) | **GET** /token | 
[**tokenVerifyGet**](AuthApi.md#tokenVerifyGet) | **GET** /token/verify | 


<a name="tokenGet"></a>
# **tokenGet**
> apiToken tokenGet()



    Gets an API token.

### Parameters
This endpoint does not need any parameter.

### Return type

[**apiToken**](../Models/apiToken.md)

### Authorization

[authToken](../README.md#authToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="tokenVerifyGet"></a>
# **tokenVerifyGet**
> tokenVerifyGet()



    Verifies the supplied API token.

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[apiToken](../README.md#apiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

