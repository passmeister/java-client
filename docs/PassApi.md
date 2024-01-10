# PassApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createOrUpdatePass**](PassApi.md#createOrUpdatePass) | **POST** /pass | This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.
[**deletePass**](PassApi.md#deletePass) | **DELETE** /pass | Delete pass by pass id.
[**getPass**](PassApi.md#getPass) | **GET** /pass | Get pass information by pass id.
[**passList**](PassApi.md#passList) | **GET** /pass/list | Retrieve the list of active pass ids for a given pass type.
[**passSync**](PassApi.md#passSync) | **POST** /pass/sync | Send updates to all active passes for a given pass type.


<a name="createOrUpdatePass"></a>
# **createOrUpdatePass**
> createOrUpdatePass(passTypeId, passId)

This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.

This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PassApi;


PassApi apiInstance = new PassApi();
Object passTypeId = null; // Object | your pass type id, for example P963493 (Urban Fitness)
Object passId = null; // Object | id of the pass (provided by you when creating the pass or automatically set by passmeister)
try {
    apiInstance.createOrUpdatePass(passTypeId, passId);
} catch (ApiException e) {
    System.err.println("Exception when calling PassApi#createOrUpdatePass");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](.md)| your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**Object**](.md)| id of the pass (provided by you when creating the pass or automatically set by passmeister) | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="deletePass"></a>
# **deletePass**
> deletePass(passTypeId, passId)

Delete pass by pass id.

Delete pass by pass id.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PassApi;


PassApi apiInstance = new PassApi();
Object passTypeId = null; // Object | your pass type id, for example P963493 (Urban Fitness)
Object passId = null; // Object | id of the pass
try {
    apiInstance.deletePass(passTypeId, passId);
} catch (ApiException e) {
    System.err.println("Exception when calling PassApi#deletePass");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](.md)| your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**Object**](.md)| id of the pass |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getPass"></a>
# **getPass**
> getPass(passTypeId, passId)

Get pass information by pass id.

Get pass information by pass id.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PassApi;


PassApi apiInstance = new PassApi();
Object passTypeId = null; // Object | your pass type id, for example P963493 (Urban Fitness)
Object passId = null; // Object | id of the pass
try {
    apiInstance.getPass(passTypeId, passId);
} catch (ApiException e) {
    System.err.println("Exception when calling PassApi#getPass");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](.md)| your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**Object**](.md)| id of the pass |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="passList"></a>
# **passList**
> passList(passTypeId, page, limit)

Retrieve the list of active pass ids for a given pass type.

Retrieve the list of active pass ids for a given pass type.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PassApi;


PassApi apiInstance = new PassApi();
Object passTypeId = null; // Object | your pass type id, for example P963493 (Urban Fitness)
Object page = null; // Object | 
Object limit = null; // Object | 
try {
    apiInstance.passList(passTypeId, page, limit);
} catch (ApiException e) {
    System.err.println("Exception when calling PassApi#passList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](.md)| your pass type id, for example P963493 (Urban Fitness) |
 **page** | [**Object**](.md)|  | [optional]
 **limit** | [**Object**](.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="passSync"></a>
# **passSync**
> passSync(passTypeId)

Send updates to all active passes for a given pass type.

For example: you changed the pass type layout and now you want to update all installed passes. (The API call only confirms the scheduling of the updates, actual updating of passes on your customers devices can take a while.)

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PassApi;


PassApi apiInstance = new PassApi();
Object passTypeId = null; // Object | your pass type id, for example P963493 (Urban Fitness)
try {
    apiInstance.passSync(passTypeId);
} catch (ApiException e) {
    System.err.println("Exception when calling PassApi#passSync");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](.md)| your pass type id, for example P963493 (Urban Fitness) |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

