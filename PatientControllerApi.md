# PatientControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findPatientByNameUsingGET**](PatientControllerApi.md#findPatientByNameUsingGET) | **GET** /patients/patient | findPatientByName
[**getPatientByIDUsingGET**](PatientControllerApi.md#getPatientByIDUsingGET) | **GET** /patients/patient/{id} | getpatientByID
[**getPatientsUsingGET**](PatientControllerApi.md#getPatientsUsingGET) | **GET** /patients | getPatients


<a name="findPatientByNameUsingGET"></a>
# **findPatientByNameUsingGET**
> String findPatientByNameUsingGET(name)

findPatientByName

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PatientControllerApi;


PatientControllerApi apiInstance = new PatientControllerApi();
String name = "eman"; // String | name
try {
    String result = apiInstance.findPatientByNameUsingGET(name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PatientControllerApi#findPatientByNameUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **String**| name | [optional] [default to eman]

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="getPatientByIDUsingGET"></a>
# **getPatientByIDUsingGET**
> PatientModelClass getPatientByIDUsingGET(id)

getpatientByID

This Operation retrievesa patient by its ID

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PatientControllerApi;


PatientControllerApi apiInstance = new PatientControllerApi();
Integer id = 56; // Integer | id
try {
    PatientModelClass result = apiInstance.getPatientByIDUsingGET(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PatientControllerApi#getPatientByIDUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| id |

### Return type

[**PatientModelClass**](PatientModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="getPatientsUsingGET"></a>
# **getPatientsUsingGET**
> List&lt;Object&gt; getPatientsUsingGET()

getPatients

This Operation retrievesall patients

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PatientControllerApi;


PatientControllerApi apiInstance = new PatientControllerApi();
try {
    List<Object> result = apiInstance.getPatientsUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PatientControllerApi#getPatientsUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**List&lt;Object&gt;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

