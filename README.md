# catalog_inventory-api-client-ruby

CatalogInventoryApiClient - the Ruby gem for the Catalog Inventory

Catalog Inventory

This SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build catalog_inventory-api-client-ruby.gemspec
```

Then either install the gem locally:

```shell
gem install ./catalog_inventory-api-client-ruby-1.0.0.gem
```

(for development, run `gem install --dev ./catalog_inventory-api-client-ruby-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'catalog_inventory-api-client-ruby', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'catalog_inventory-api-client-ruby', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:

```ruby
# Load the gem
require 'catalog_inventory-api-client-ruby'

# Setup authorization
CatalogInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR_USERNAME'
  config.password = 'YOUR_PASSWORD'
end

api_instance = CatalogInventoryApiClient::DefaultApi.new

begin
  #Return this API document in JSON format
  result = api_instance.get_documentation
  p result
rescue CatalogInventoryApiClient::ApiError => e
  puts "Exception when calling DefaultApi->get_documentation: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *https://cloud.redhat.com//api/catalog-inventory/v1.0*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CatalogInventoryApiClient::DefaultApi* | [**get_documentation**](docs/DefaultApi.md#get_documentation) | **GET** /openapi.json | Return this API document in JSON format
*CatalogInventoryApiClient::DefaultApi* | [**post_graph_ql**](docs/DefaultApi.md#post_graph_ql) | **POST** /graphql | Perform a GraphQL Query
*CatalogInventoryApiClient::ServiceCredentialApi* | [**list_service_credentials**](docs/ServiceCredentialApi.md#list_service_credentials) | **GET** /service_credentials | List ServiceCredentials
*CatalogInventoryApiClient::ServiceCredentialApi* | [**show_service_credential**](docs/ServiceCredentialApi.md#show_service_credential) | **GET** /service_credentials/{id} | Show an existing ServiceCredential
*CatalogInventoryApiClient::ServiceCredentialTypeApi* | [**list_service_credential_types**](docs/ServiceCredentialTypeApi.md#list_service_credential_types) | **GET** /service_credential_types | List ServiceCredentialTypes
*CatalogInventoryApiClient::ServiceCredentialTypeApi* | [**show_service_credential_type**](docs/ServiceCredentialTypeApi.md#show_service_credential_type) | **GET** /service_credential_types/{id} | Show an existing ServiceCredentialType
*CatalogInventoryApiClient::ServiceInstanceApi* | [**list_service_instance_service_credentials**](docs/ServiceInstanceApi.md#list_service_instance_service_credentials) | **GET** /service_instances/{id}/service_credentials | List ServiceCredentials for ServiceInstance
*CatalogInventoryApiClient::ServiceInstanceApi* | [**list_service_instance_service_instance_nodes**](docs/ServiceInstanceApi.md#list_service_instance_service_instance_nodes) | **GET** /service_instances/{id}/service_instance_nodes | List ServiceInstanceNodes for ServiceInstance
*CatalogInventoryApiClient::ServiceInstanceApi* | [**list_service_instances**](docs/ServiceInstanceApi.md#list_service_instances) | **GET** /service_instances | List ServiceInstances
*CatalogInventoryApiClient::ServiceInstanceApi* | [**show_service_instance**](docs/ServiceInstanceApi.md#show_service_instance) | **GET** /service_instances/{id} | Show an existing ServiceInstance
*CatalogInventoryApiClient::ServiceInstanceNodeApi* | [**list_service_instance_node_service_credentials**](docs/ServiceInstanceNodeApi.md#list_service_instance_node_service_credentials) | **GET** /service_instance_nodes/{id}/service_credentials | List ServiceCredentials for ServiceInstanceNode
*CatalogInventoryApiClient::ServiceInstanceNodeApi* | [**list_service_instance_nodes**](docs/ServiceInstanceNodeApi.md#list_service_instance_nodes) | **GET** /service_instance_nodes | List ServiceInstanceNodes
*CatalogInventoryApiClient::ServiceInstanceNodeApi* | [**show_service_instance_node**](docs/ServiceInstanceNodeApi.md#show_service_instance_node) | **GET** /service_instance_nodes/{id} | Show an existing ServiceInstanceNode
*CatalogInventoryApiClient::ServiceInventoryApi* | [**list_service_inventories**](docs/ServiceInventoryApi.md#list_service_inventories) | **GET** /service_inventories | List ServiceInventories
*CatalogInventoryApiClient::ServiceInventoryApi* | [**list_service_inventory_tags**](docs/ServiceInventoryApi.md#list_service_inventory_tags) | **GET** /service_inventories/{id}/tags | List Tags for ServiceInventory
*CatalogInventoryApiClient::ServiceInventoryApi* | [**show_service_inventory**](docs/ServiceInventoryApi.md#show_service_inventory) | **GET** /service_inventories/{id} | Show an existing ServiceInventory
*CatalogInventoryApiClient::ServiceInventoryApi* | [**tag_service_inventory**](docs/ServiceInventoryApi.md#tag_service_inventory) | **POST** /service_inventories/{id}/tag | Tag a ServiceInventory
*CatalogInventoryApiClient::ServiceInventoryApi* | [**untag_service_inventory**](docs/ServiceInventoryApi.md#untag_service_inventory) | **POST** /service_inventories/{id}/untag | Untag a ServiceInventory
*CatalogInventoryApiClient::ServiceOfferingApi* | [**applied_inventories_tags_for_service_offering**](docs/ServiceOfferingApi.md#applied_inventories_tags_for_service_offering) | **POST** /service_offerings/{id}/applied_inventories_tags | Invokes computing of ServiceInventories tags for given ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offering_service_credentials**](docs/ServiceOfferingApi.md#list_service_offering_service_credentials) | **GET** /service_offerings/{id}/service_credentials | List ServiceCredentials for ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offering_service_instances**](docs/ServiceOfferingApi.md#list_service_offering_service_instances) | **GET** /service_offerings/{id}/service_instances | List ServiceInstances for ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offering_service_offering_nodes**](docs/ServiceOfferingApi.md#list_service_offering_service_offering_nodes) | **GET** /service_offerings/{id}/service_offering_nodes | List ServiceOfferingNodes for ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offering_service_plans**](docs/ServiceOfferingApi.md#list_service_offering_service_plans) | **GET** /service_offerings/{id}/service_plans | List ServicePlans for ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offering_tags**](docs/ServiceOfferingApi.md#list_service_offering_tags) | **GET** /service_offerings/{id}/tags | List Tags for ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**list_service_offerings**](docs/ServiceOfferingApi.md#list_service_offerings) | **GET** /service_offerings | List ServiceOfferings
*CatalogInventoryApiClient::ServiceOfferingApi* | [**order_service_offering**](docs/ServiceOfferingApi.md#order_service_offering) | **POST** /service_offerings/{id}/order | Order an existing ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**show_service_offering**](docs/ServiceOfferingApi.md#show_service_offering) | **GET** /service_offerings/{id} | Show an existing ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**tag_service_offering**](docs/ServiceOfferingApi.md#tag_service_offering) | **POST** /service_offerings/{id}/tag | Tag a ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingApi* | [**untag_service_offering**](docs/ServiceOfferingApi.md#untag_service_offering) | **POST** /service_offerings/{id}/untag | Untag a ServiceOffering
*CatalogInventoryApiClient::ServiceOfferingIconApi* | [**list_service_offering_icons**](docs/ServiceOfferingIconApi.md#list_service_offering_icons) | **GET** /service_offering_icons | List ServiceOfferingIcons
*CatalogInventoryApiClient::ServiceOfferingIconApi* | [**show_service_offering_icon**](docs/ServiceOfferingIconApi.md#show_service_offering_icon) | **GET** /service_offering_icons/{id} | Show an existing ServiceOfferingIcon
*CatalogInventoryApiClient::ServiceOfferingIconApi* | [**show_service_offering_icon_icon_data**](docs/ServiceOfferingIconApi.md#show_service_offering_icon_icon_data) | **GET** /service_offering_icons/{id}/icon_data | Show an existing ServiceOfferingIcon IconData
*CatalogInventoryApiClient::ServiceOfferingNodeApi* | [**list_service_offering_node_service_credentials**](docs/ServiceOfferingNodeApi.md#list_service_offering_node_service_credentials) | **GET** /service_offering_nodes/{id}/service_credentials | List ServiceCredentials for ServiceOfferingNode
*CatalogInventoryApiClient::ServiceOfferingNodeApi* | [**list_service_offering_nodes**](docs/ServiceOfferingNodeApi.md#list_service_offering_nodes) | **GET** /service_offering_nodes | List ServiceOfferingNodes
*CatalogInventoryApiClient::ServiceOfferingNodeApi* | [**show_service_offering_node**](docs/ServiceOfferingNodeApi.md#show_service_offering_node) | **GET** /service_offering_nodes/{id} | Show an existing ServiceOfferingNode
*CatalogInventoryApiClient::ServicePlanApi* | [**list_service_plan_service_instances**](docs/ServicePlanApi.md#list_service_plan_service_instances) | **GET** /service_plans/{id}/service_instances | List ServiceInstances for ServicePlan
*CatalogInventoryApiClient::ServicePlanApi* | [**list_service_plans**](docs/ServicePlanApi.md#list_service_plans) | **GET** /service_plans | List ServicePlans
*CatalogInventoryApiClient::ServicePlanApi* | [**order_service_plan**](docs/ServicePlanApi.md#order_service_plan) | **POST** /service_plans/{id}/order | Order an existing ServicePlan
*CatalogInventoryApiClient::ServicePlanApi* | [**show_service_plan**](docs/ServicePlanApi.md#show_service_plan) | **GET** /service_plans/{id} | Show an existing ServicePlan
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_instance_nodes**](docs/SourceApi.md#list_source_service_instance_nodes) | **GET** /sources/{id}/service_instance_nodes | List ServiceInstanceNodes for Source
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_instances**](docs/SourceApi.md#list_source_service_instances) | **GET** /sources/{id}/service_instances | List ServiceInstances for Source
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_inventories**](docs/SourceApi.md#list_source_service_inventories) | **GET** /sources/{id}/service_inventories | List ServiceInventories for Source
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_offering_nodes**](docs/SourceApi.md#list_source_service_offering_nodes) | **GET** /sources/{id}/service_offering_nodes | List ServiceOfferingNodes for Source
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_offerings**](docs/SourceApi.md#list_source_service_offerings) | **GET** /sources/{id}/service_offerings | List ServiceOfferings for Source
*CatalogInventoryApiClient::SourceApi* | [**list_source_service_plans**](docs/SourceApi.md#list_source_service_plans) | **GET** /sources/{id}/service_plans | List ServicePlans for Source
*CatalogInventoryApiClient::SourceApi* | [**list_sources**](docs/SourceApi.md#list_sources) | **GET** /sources | List Sources
*CatalogInventoryApiClient::SourceApi* | [**show_source**](docs/SourceApi.md#show_source) | **GET** /sources/{id} | Show an existing Source
*CatalogInventoryApiClient::TagsApi* | [**list_tag_service_inventories**](docs/TagsApi.md#list_tag_service_inventories) | **GET** /tags/{id}/service_inventories | List ServiceInventories for Tag
*CatalogInventoryApiClient::TagsApi* | [**list_tag_service_offerings**](docs/TagsApi.md#list_tag_service_offerings) | **GET** /tags/{id}/service_offerings | List ServiceOfferings for Tag
*CatalogInventoryApiClient::TagsApi* | [**list_tags**](docs/TagsApi.md#list_tags) | **GET** /tags | List Tags
*CatalogInventoryApiClient::TagsApi* | [**show_tag**](docs/TagsApi.md#show_tag) | **GET** /tags/{id} | Show an existing Tag
*CatalogInventoryApiClient::TaskApi* | [**list_tasks**](docs/TaskApi.md#list_tasks) | **GET** /tasks | List Tasks
*CatalogInventoryApiClient::TaskApi* | [**show_task**](docs/TaskApi.md#show_task) | **GET** /tasks/{id} | Show an existing Task
*CatalogInventoryApiClient::TaskApi* | [**update_task**](docs/TaskApi.md#update_task) | **PATCH** /tasks/{id} | Update an existing Task


## Documentation for Models

 - [CatalogInventoryApiClient::AppliedInventoriesParametersServicePlan](docs/AppliedInventoriesParametersServicePlan.md)
 - [CatalogInventoryApiClient::CheckAvailabilityTask](docs/CheckAvailabilityTask.md)
 - [CatalogInventoryApiClient::CollectionLinks](docs/CollectionLinks.md)
 - [CatalogInventoryApiClient::CollectionMetadata](docs/CollectionMetadata.md)
 - [CatalogInventoryApiClient::ErrorNotFound](docs/ErrorNotFound.md)
 - [CatalogInventoryApiClient::ErrorNotFoundErrors](docs/ErrorNotFoundErrors.md)
 - [CatalogInventoryApiClient::FullRefreshPersisterTask](docs/FullRefreshPersisterTask.md)
 - [CatalogInventoryApiClient::FullRefreshUploadTask](docs/FullRefreshUploadTask.md)
 - [CatalogInventoryApiClient::GraphQLRequest](docs/GraphQLRequest.md)
 - [CatalogInventoryApiClient::GraphQLResponse](docs/GraphQLResponse.md)
 - [CatalogInventoryApiClient::IncrementalRefreshUploadTask](docs/IncrementalRefreshUploadTask.md)
 - [CatalogInventoryApiClient::InlineResponse200](docs/InlineResponse200.md)
 - [CatalogInventoryApiClient::LaunchJobTask](docs/LaunchJobTask.md)
 - [CatalogInventoryApiClient::OrderParametersServiceOffering](docs/OrderParametersServiceOffering.md)
 - [CatalogInventoryApiClient::OrderParametersServicePlan](docs/OrderParametersServicePlan.md)
 - [CatalogInventoryApiClient::ServiceCredential](docs/ServiceCredential.md)
 - [CatalogInventoryApiClient::ServiceCredentialType](docs/ServiceCredentialType.md)
 - [CatalogInventoryApiClient::ServiceCredentialTypesCollection](docs/ServiceCredentialTypesCollection.md)
 - [CatalogInventoryApiClient::ServiceCredentialsCollection](docs/ServiceCredentialsCollection.md)
 - [CatalogInventoryApiClient::ServiceInstance](docs/ServiceInstance.md)
 - [CatalogInventoryApiClient::ServiceInstanceNode](docs/ServiceInstanceNode.md)
 - [CatalogInventoryApiClient::ServiceInstanceNodesCollection](docs/ServiceInstanceNodesCollection.md)
 - [CatalogInventoryApiClient::ServiceInstancesCollection](docs/ServiceInstancesCollection.md)
 - [CatalogInventoryApiClient::ServiceInventoriesCollection](docs/ServiceInventoriesCollection.md)
 - [CatalogInventoryApiClient::ServiceInventory](docs/ServiceInventory.md)
 - [CatalogInventoryApiClient::ServiceOffering](docs/ServiceOffering.md)
 - [CatalogInventoryApiClient::ServiceOfferingIcon](docs/ServiceOfferingIcon.md)
 - [CatalogInventoryApiClient::ServiceOfferingIconsCollection](docs/ServiceOfferingIconsCollection.md)
 - [CatalogInventoryApiClient::ServiceOfferingNode](docs/ServiceOfferingNode.md)
 - [CatalogInventoryApiClient::ServiceOfferingNodesCollection](docs/ServiceOfferingNodesCollection.md)
 - [CatalogInventoryApiClient::ServiceOfferingsCollection](docs/ServiceOfferingsCollection.md)
 - [CatalogInventoryApiClient::ServicePlan](docs/ServicePlan.md)
 - [CatalogInventoryApiClient::ServicePlansCollection](docs/ServicePlansCollection.md)
 - [CatalogInventoryApiClient::Source](docs/Source.md)
 - [CatalogInventoryApiClient::SourcesCollection](docs/SourcesCollection.md)
 - [CatalogInventoryApiClient::Tag](docs/Tag.md)
 - [CatalogInventoryApiClient::TagsCollection](docs/TagsCollection.md)
 - [CatalogInventoryApiClient::Task](docs/Task.md)
 - [CatalogInventoryApiClient::TasksCollection](docs/TasksCollection.md)
 - [CatalogInventoryApiClient::Tenant](docs/Tenant.md)


## Documentation for Authorization


### UserSecurity

- **Type**: HTTP basic authentication

