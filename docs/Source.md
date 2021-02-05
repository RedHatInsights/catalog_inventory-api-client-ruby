# CatalogInventoryApiClient::Source

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**archived_at** | **DateTime** |  | [optional] [readonly] 
**created_at** | **DateTime** |  | [optional] [readonly] 
**id** | **String** | ID of the resource | [optional] [readonly] 
**info** | [**Object**](.md) |  | [optional] [readonly] 
**name** | **String** |  | [optional] [readonly] 
**mqtt_client_id** | **String** |  | [optional] [readonly] 
**enabled** | **Boolean** |  | [optional] [readonly] [default to false]
**refresh_state** | **String** |  | [optional] 
**bytes_received** | **Integer** |  | [optional] 
**bytes_sent** | **Integer** |  | [optional] 
**refresh_started_at** | **DateTime** |  | [optional] [readonly] 
**refresh_finished_at** | **DateTime** |  | [optional] [readonly] 
**availability_status** | **String** |  | [optional] 
**last_successful_refresh_at** | **DateTime** |  | [optional] [readonly] 
**last_checked_at** | **DateTime** |  | [optional] [readonly] 
**last_available_at** | **DateTime** |  | [optional] [readonly] 
**uid** | **String** |  | [optional] [readonly] 
**updated_at** | **DateTime** |  | [optional] [readonly] 

## Code Sample

```ruby
require 'CatalogInventoryApiClient'

instance = CatalogInventoryApiClient::Source.new(archived_at: null,
                                 created_at: null,
                                 id: null,
                                 info: The version of Tower being used,
                                 name: The Source Name,
                                 mqtt_client_id: The GUID of MQTT client being used,
                                 enabled: null,
                                 refresh_state: null,
                                 bytes_received: null,
                                 bytes_sent: null,
                                 refresh_started_at: null,
                                 refresh_finished_at: null,
                                 availability_status: The availability status of source,
                                 last_successful_refresh_at: null,
                                 last_checked_at: null,
                                 last_available_at: null,
                                 uid: null,
                                 updated_at: null)
```


