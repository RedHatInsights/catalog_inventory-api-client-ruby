# CatalogInventoryApiClient::OrderParametersServicePlan

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**service_parameters** | [**Object**](.md) | JSON object with provisioning parameters | [optional] 
**provider_control_parameters** | [**Object**](.md) | The provider specific parameters needed to provision this service. This might include namespaces, special keys | [optional] 

## Code Sample

```ruby
require 'CatalogInventoryApiClient'

instance = CatalogInventoryApiClient::OrderParametersServicePlan.new(service_parameters: null,
                                 provider_control_parameters: null)
```


