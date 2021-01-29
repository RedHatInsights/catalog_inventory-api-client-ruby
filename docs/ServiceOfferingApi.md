# CatalogInventoryApiClient::ServiceOfferingApi

All URIs are relative to *https://cloud.redhat.com//api/catalog-inventory/v1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applied_inventories_tags_for_service_offering**](ServiceOfferingApi.md#applied_inventories_tags_for_service_offering) | **POST** /service_offerings/{id}/applied_inventories_tags | Invokes computing of ServiceInventories tags for given ServiceOffering
[**list_service_offering_service_credentials**](ServiceOfferingApi.md#list_service_offering_service_credentials) | **GET** /service_offerings/{id}/service_credentials | List ServiceCredentials for ServiceOffering
[**list_service_offering_service_instances**](ServiceOfferingApi.md#list_service_offering_service_instances) | **GET** /service_offerings/{id}/service_instances | List ServiceInstances for ServiceOffering
[**list_service_offering_service_offering_nodes**](ServiceOfferingApi.md#list_service_offering_service_offering_nodes) | **GET** /service_offerings/{id}/service_offering_nodes | List ServiceOfferingNodes for ServiceOffering
[**list_service_offering_service_plans**](ServiceOfferingApi.md#list_service_offering_service_plans) | **GET** /service_offerings/{id}/service_plans | List ServicePlans for ServiceOffering
[**list_service_offering_tags**](ServiceOfferingApi.md#list_service_offering_tags) | **GET** /service_offerings/{id}/tags | List Tags for ServiceOffering
[**list_service_offerings**](ServiceOfferingApi.md#list_service_offerings) | **GET** /service_offerings | List ServiceOfferings
[**order_service_offering**](ServiceOfferingApi.md#order_service_offering) | **POST** /service_offerings/{id}/order | Order an existing ServiceOffering
[**show_service_offering**](ServiceOfferingApi.md#show_service_offering) | **GET** /service_offerings/{id} | Show an existing ServiceOffering
[**tag_service_offering**](ServiceOfferingApi.md#tag_service_offering) | **POST** /service_offerings/{id}/tag | Tag a ServiceOffering
[**untag_service_offering**](ServiceOfferingApi.md#untag_service_offering) | **POST** /service_offerings/{id}/untag | Untag a ServiceOffering



## applied_inventories_tags_for_service_offering

> Array&lt;Tag&gt; applied_inventories_tags_for_service_offering(id, applied_inventories_parameters_service_plan)

Invokes computing of ServiceInventories tags for given ServiceOffering

Returns an array of inventories tags

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
applied_inventories_parameters_service_plan = CatalogInventoryApiClient::AppliedInventoriesParametersServicePlan.new # AppliedInventoriesParametersServicePlan | Parameters defining input data for computing inventories

begin
  #Invokes computing of ServiceInventories tags for given ServiceOffering
  result = api_instance.applied_inventories_tags_for_service_offering(id, applied_inventories_parameters_service_plan)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->applied_inventories_tags_for_service_offering: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **applied_inventories_parameters_service_plan** | [**AppliedInventoriesParametersServicePlan**](AppliedInventoriesParametersServicePlan.md)| Parameters defining input data for computing inventories | 

### Return type

[**Array&lt;Tag&gt;**](Tag.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## list_service_offering_service_credentials

> ServiceCredentialsCollection list_service_offering_service_credentials(id, opts)

List ServiceCredentials for ServiceOffering

Returns an array of ServiceCredential objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List ServiceCredentials for ServiceOffering
  result = api_instance.list_service_offering_service_credentials(id, opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offering_service_credentials: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**ServiceCredentialsCollection**](ServiceCredentialsCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_service_offering_service_instances

> ServiceInstancesCollection list_service_offering_service_instances(id, opts)

List ServiceInstances for ServiceOffering

Returns an array of ServiceInstance objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List ServiceInstances for ServiceOffering
  result = api_instance.list_service_offering_service_instances(id, opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offering_service_instances: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**ServiceInstancesCollection**](ServiceInstancesCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_service_offering_service_offering_nodes

> ServiceOfferingNodesCollection list_service_offering_service_offering_nodes(id, opts)

List ServiceOfferingNodes for ServiceOffering

Returns an array of ServiceOfferingNode objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List ServiceOfferingNodes for ServiceOffering
  result = api_instance.list_service_offering_service_offering_nodes(id, opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offering_service_offering_nodes: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**ServiceOfferingNodesCollection**](ServiceOfferingNodesCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_service_offering_service_plans

> ServicePlansCollection list_service_offering_service_plans(id, opts)

List ServicePlans for ServiceOffering

Returns an array of ServicePlan objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List ServicePlans for ServiceOffering
  result = api_instance.list_service_offering_service_plans(id, opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offering_service_plans: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**ServicePlansCollection**](ServicePlansCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_service_offering_tags

> TagsCollection list_service_offering_tags(id, opts)

List Tags for ServiceOffering

Returns an array of Tag objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List Tags for ServiceOffering
  result = api_instance.list_service_offering_tags(id, opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offering_tags: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**TagsCollection**](TagsCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_service_offerings

> ServiceOfferingsCollection list_service_offerings(opts)

List ServiceOfferings

Returns an array of ServiceOffering objects

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
opts = {
  limit: 100, # Integer | The numbers of items to return per page.
  offset: 0, # Integer | The number of items to skip before starting to collect the result set.
  filter: nil, # Object | Filter for querying collections.
  sort_by: nil # Object | The list of attribute and order to sort the result set by.
}

begin
  #List ServiceOfferings
  result = api_instance.list_service_offerings(opts)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->list_service_offerings: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **Integer**| The numbers of items to return per page. | [optional] [default to 100]
 **offset** | **Integer**| The number of items to skip before starting to collect the result set. | [optional] [default to 0]
 **filter** | [**Object**](.md)| Filter for querying collections. | [optional] 
 **sort_by** | [**Object**](.md)| The list of attribute and order to sort the result set by. | [optional] 

### Return type

[**ServiceOfferingsCollection**](ServiceOfferingsCollection.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## order_service_offering

> InlineResponse200 order_service_offering(id, order_parameters_service_offering)

Order an existing ServiceOffering

Returns a Task id

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
order_parameters_service_offering = CatalogInventoryApiClient::OrderParametersServiceOffering.new # OrderParametersServiceOffering | Order parameters defining the service and provider control

begin
  #Order an existing ServiceOffering
  result = api_instance.order_service_offering(id, order_parameters_service_offering)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->order_service_offering: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **order_parameters_service_offering** | [**OrderParametersServiceOffering**](OrderParametersServiceOffering.md)| Order parameters defining the service and provider control | 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## show_service_offering

> ServiceOffering show_service_offering(id)

Show an existing ServiceOffering

Returns a ServiceOffering object

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource

begin
  #Show an existing ServiceOffering
  result = api_instance.show_service_offering(id)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->show_service_offering: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 

### Return type

[**ServiceOffering**](ServiceOffering.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## tag_service_offering

> Array&lt;Tag&gt; tag_service_offering(id, tag)

Tag a ServiceOffering

Tags a ServiceOffering object

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
tag = [CatalogInventoryApiClient::Tag.new] # Array<Tag> | Tag attributes to add

begin
  #Tag a ServiceOffering
  result = api_instance.tag_service_offering(id, tag)
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->tag_service_offering: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **tag** | [**Array&lt;Tag&gt;**](Tag.md)| Tag attributes to add | 

### Return type

[**Array&lt;Tag&gt;**](Tag.md)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## untag_service_offering

> untag_service_offering(id, tag)

Untag a ServiceOffering

Untags a ServiceOffering object

### Example

```ruby
# load the gem
require 'catalog_inventory-api-client-ruby'
# setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = CatalogInventoryApiClient::ServiceOfferingApi.new
id = 'id_example' # String | ID of the resource
tag = [CatalogInventoryApiClient::Tag.new] # Array<Tag> | Tag attributes to removed

begin
  #Untag a ServiceOffering
  api_instance.untag_service_offering(id, tag)
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling ServiceOfferingApi->untag_service_offering: #{e}"
end
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| ID of the resource | 
 **tag** | [**Array&lt;Tag&gt;**](Tag.md)| Tag attributes to removed | 

### Return type

nil (empty response body)

### Authorization

[UserSecurity](../README.md#UserSecurity)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

