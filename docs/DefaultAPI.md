# \DefaultAPI

All URIs are relative to *https://api.ipdetective.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetBulkIP**](DefaultAPI.md#GetBulkIP) | **Post** /ip | Bulk IP Lookup
[**GetIP**](DefaultAPI.md#GetIP) | **Get** /ip/{ip} | Single IP Lookup
[**GetMyIP**](DefaultAPI.md#GetMyIP) | **Get** /ip | My IP
[**GetUsage**](DefaultAPI.md#GetUsage) | **Get** /usage | API Usage



## GetBulkIP

> []IPResponse GetBulkIP(ctx).RequestBody(requestBody).Info(info).Execute()

Bulk IP Lookup



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	ipdetective "github.com/AndrewCopeland/go-ipdetective"
)

func main() {
	requestBody := []string{"Property_example"} // []string | 
	info := true // bool | If true, returns additional info like country and ASN for each IP. (optional)

	configuration := ipdetective.NewConfiguration()
	apiClient := ipdetective.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetBulkIP(context.Background()).RequestBody(requestBody).Info(info).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetBulkIP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBulkIP`: []IPResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetBulkIP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetBulkIPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requestBody** | **[]string** |  | 
 **info** | **bool** | If true, returns additional info like country and ASN for each IP. | 

### Return type

[**[]IPResponse**](IPResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetIP

> IPResponse GetIP(ctx, ip).Info(info).Execute()

Single IP Lookup



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	ipdetective "github.com/AndrewCopeland/go-ipdetective"
)

func main() {
	ip := "8.8.8.8" // string | 
	info := true // bool | If true, returns additional info like country and ASN. (optional)

	configuration := ipdetective.NewConfiguration()
	apiClient := ipdetective.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetIP(context.Background(), ip).Info(info).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetIP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetIP`: IPResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetIP`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ip** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetIPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **info** | **bool** | If true, returns additional info like country and ASN. | 

### Return type

[**IPResponse**](IPResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMyIP

> IPResponse GetMyIP(ctx).Info(info).Execute()

My IP



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	ipdetective "github.com/AndrewCopeland/go-ipdetective"
)

func main() {
	info := true // bool | If true, returns additional info like country and ASN. (optional)

	configuration := ipdetective.NewConfiguration()
	apiClient := ipdetective.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetMyIP(context.Background()).Info(info).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetMyIP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMyIP`: IPResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetMyIP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetMyIPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **info** | **bool** | If true, returns additional info like country and ASN. | 

### Return type

[**IPResponse**](IPResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUsage

> UsageResponse GetUsage(ctx).Execute()

API Usage



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	ipdetective "github.com/AndrewCopeland/go-ipdetective"
)

func main() {

	configuration := ipdetective.NewConfiguration()
	apiClient := ipdetective.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetUsage(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetUsage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUsage`: UsageResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetUsage`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUsageRequest struct via the builder pattern


### Return type

[**UsageResponse**](UsageResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

