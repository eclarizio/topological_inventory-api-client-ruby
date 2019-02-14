# topological_inventory-api-client

TopologicalInventoryApiClient - the Ruby gem for the Topological Inventory

Topological Inventory

This SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 0.1.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build topological_inventory-api-client.gemspec
```

Then either install the gem locally:

```shell
gem install ./topological_inventory-api-client-1.0.0.gem
```
(for development, run `gem install --dev ./topological_inventory-api-client-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'topological_inventory-api-client', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'topological_inventory-api-client', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:
```ruby
# Load the gem
require 'topological_inventory-api-client'

# Setup authorization
TopologicalInventoryApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = TopologicalInventoryApiClient::DefaultApi.new
authentication = TopologicalInventoryApiClient::Authentication.new # Authentication | Authentication attributes to create

begin
  #Create a new Authentication
  result = api_instance.create_authentication(authentication)
  p result
rescue TopologicalInventoryApiClient::ApiError => e
  puts "Exception when calling DefaultApi->create_authentication: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *https://virtserver.swaggerhub.com/r/insights/platform/topological-inventory/v0.1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*TopologicalInventoryApiClient::DefaultApi* | [**create_authentication**](docs/DefaultApi.md#create_authentication) | **POST** /authentications | Create a new Authentication
*TopologicalInventoryApiClient::DefaultApi* | [**create_endpoint**](docs/DefaultApi.md#create_endpoint) | **POST** /endpoints | Create a new Endpoint
*TopologicalInventoryApiClient::DefaultApi* | [**create_source**](docs/DefaultApi.md#create_source) | **POST** /sources | Create a new Source
*TopologicalInventoryApiClient::DefaultApi* | [**create_source_type**](docs/DefaultApi.md#create_source_type) | **POST** /source_types | Create a new SourceType
*TopologicalInventoryApiClient::DefaultApi* | [**delete_authentication**](docs/DefaultApi.md#delete_authentication) | **DELETE** /authentications/{id} | Delete an existing Authentication
*TopologicalInventoryApiClient::DefaultApi* | [**delete_endpoint**](docs/DefaultApi.md#delete_endpoint) | **DELETE** /endpoints/{id} | Delete an existing Endpoint
*TopologicalInventoryApiClient::DefaultApi* | [**delete_source**](docs/DefaultApi.md#delete_source) | **DELETE** /sources/{id} | Delete an existing Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_authentications**](docs/DefaultApi.md#list_authentications) | **GET** /authentications | List Authentications
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_group_containers**](docs/DefaultApi.md#list_container_group_containers) | **GET** /container_groups/{id}/containers | List Containers for ContainerGroup
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_groups**](docs/DefaultApi.md#list_container_groups) | **GET** /container_groups | List ContainerGroups
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_images**](docs/DefaultApi.md#list_container_images) | **GET** /container_images | List ContainerImages
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_node_container_groups**](docs/DefaultApi.md#list_container_node_container_groups) | **GET** /container_nodes/{id}/container_groups | List ContainerGroups for ContainerNode
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_nodes**](docs/DefaultApi.md#list_container_nodes) | **GET** /container_nodes | List ContainerNodes
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_project_container_groups**](docs/DefaultApi.md#list_container_project_container_groups) | **GET** /container_projects/{id}/container_groups | List ContainerGroups for ContainerProject
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_project_container_templates**](docs/DefaultApi.md#list_container_project_container_templates) | **GET** /container_projects/{id}/container_templates | List ContainerTemplates for ContainerProject
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_projects**](docs/DefaultApi.md#list_container_projects) | **GET** /container_projects | List ContainerProjects
*TopologicalInventoryApiClient::DefaultApi* | [**list_container_templates**](docs/DefaultApi.md#list_container_templates) | **GET** /container_templates | List ContainerTemplates
*TopologicalInventoryApiClient::DefaultApi* | [**list_containers**](docs/DefaultApi.md#list_containers) | **GET** /containers | List Containers
*TopologicalInventoryApiClient::DefaultApi* | [**list_endpoint_authentications**](docs/DefaultApi.md#list_endpoint_authentications) | **GET** /endpoints/{id}/authentications | List Authentications for Endpoint
*TopologicalInventoryApiClient::DefaultApi* | [**list_endpoints**](docs/DefaultApi.md#list_endpoints) | **GET** /endpoints | List Endpoints
*TopologicalInventoryApiClient::DefaultApi* | [**list_flavors**](docs/DefaultApi.md#list_flavors) | **GET** /flavors | List Flavors
*TopologicalInventoryApiClient::DefaultApi* | [**list_orchestration_stacks**](docs/DefaultApi.md#list_orchestration_stacks) | **GET** /orchestration_stacks | List OrchestrationStacks
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_instances**](docs/DefaultApi.md#list_service_instances) | **GET** /service_instances | List ServiceInstances
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_offering_icons**](docs/DefaultApi.md#list_service_offering_icons) | **GET** /service_offering_icons | List ServiceOfferingIcons
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_offering_service_instances**](docs/DefaultApi.md#list_service_offering_service_instances) | **GET** /service_offerings/{id}/service_instances | List ServiceInstances for ServiceOffering
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_offering_service_plans**](docs/DefaultApi.md#list_service_offering_service_plans) | **GET** /service_offerings/{id}/service_plans | List ServicePlans for ServiceOffering
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_offerings**](docs/DefaultApi.md#list_service_offerings) | **GET** /service_offerings | List ServiceOfferings
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_plan_service_instances**](docs/DefaultApi.md#list_service_plan_service_instances) | **GET** /service_plans/{id}/service_instances | List ServiceInstances for ServicePlan
*TopologicalInventoryApiClient::DefaultApi* | [**list_service_plans**](docs/DefaultApi.md#list_service_plans) | **GET** /service_plans | List ServicePlans
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_container_groups**](docs/DefaultApi.md#list_source_container_groups) | **GET** /sources/{id}/container_groups | List ContainerGroups for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_container_images**](docs/DefaultApi.md#list_source_container_images) | **GET** /sources/{id}/container_images | List ContainerImages for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_container_nodes**](docs/DefaultApi.md#list_source_container_nodes) | **GET** /sources/{id}/container_nodes | List ContainerNodes for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_container_projects**](docs/DefaultApi.md#list_source_container_projects) | **GET** /sources/{id}/container_projects | List ContainerProjects for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_container_templates**](docs/DefaultApi.md#list_source_container_templates) | **GET** /sources/{id}/container_templates | List ContainerTemplates for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_containers**](docs/DefaultApi.md#list_source_containers) | **GET** /sources/{id}/containers | List Containers for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_endpoints**](docs/DefaultApi.md#list_source_endpoints) | **GET** /sources/{id}/endpoints | List Endpoints for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_orchestration_stacks**](docs/DefaultApi.md#list_source_orchestration_stacks) | **GET** /sources/{id}/orchestration_stacks | List OrchestrationStacks for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_service_instances**](docs/DefaultApi.md#list_source_service_instances) | **GET** /sources/{id}/service_instances | List ServiceInstances for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_service_offerings**](docs/DefaultApi.md#list_source_service_offerings) | **GET** /sources/{id}/service_offerings | List ServiceOfferings for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_service_plans**](docs/DefaultApi.md#list_source_service_plans) | **GET** /sources/{id}/service_plans | List ServicePlans for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_type_sources**](docs/DefaultApi.md#list_source_type_sources) | **GET** /source_types/{id}/sources | List Sources for SourceType
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_types**](docs/DefaultApi.md#list_source_types) | **GET** /source_types | List SourceTypes
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_vms**](docs/DefaultApi.md#list_source_vms) | **GET** /sources/{id}/vms | List Vms for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_volume_types**](docs/DefaultApi.md#list_source_volume_types) | **GET** /sources/{id}/volume_types | List VolumeTypes for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_source_volumes**](docs/DefaultApi.md#list_source_volumes) | **GET** /sources/{id}/volumes | List Volumes for Source
*TopologicalInventoryApiClient::DefaultApi* | [**list_sources**](docs/DefaultApi.md#list_sources) | **GET** /sources | List Sources
*TopologicalInventoryApiClient::DefaultApi* | [**list_tags**](docs/DefaultApi.md#list_tags) | **GET** /tags | List Tags
*TopologicalInventoryApiClient::DefaultApi* | [**list_tasks**](docs/DefaultApi.md#list_tasks) | **GET** /tasks | List Tasks
*TopologicalInventoryApiClient::DefaultApi* | [**list_vm_volume_attachments**](docs/DefaultApi.md#list_vm_volume_attachments) | **GET** /vms/{id}/volume_attachments | List VolumeAttachments for Vm
*TopologicalInventoryApiClient::DefaultApi* | [**list_vm_volumes**](docs/DefaultApi.md#list_vm_volumes) | **GET** /vms/{id}/volumes | List Volumes for Vm
*TopologicalInventoryApiClient::DefaultApi* | [**list_vms**](docs/DefaultApi.md#list_vms) | **GET** /vms | List Vms
*TopologicalInventoryApiClient::DefaultApi* | [**list_volume_attachments**](docs/DefaultApi.md#list_volume_attachments) | **GET** /volume_attachments | List VolumeAttachments
*TopologicalInventoryApiClient::DefaultApi* | [**list_volume_types**](docs/DefaultApi.md#list_volume_types) | **GET** /volume_types | List VolumeTypes
*TopologicalInventoryApiClient::DefaultApi* | [**list_volumes**](docs/DefaultApi.md#list_volumes) | **GET** /volumes | List Volumes
*TopologicalInventoryApiClient::DefaultApi* | [**order_service_plan**](docs/DefaultApi.md#order_service_plan) | **POST** /service_plans/{id}/order | Order an existing ServicePlan
*TopologicalInventoryApiClient::DefaultApi* | [**show_authentication**](docs/DefaultApi.md#show_authentication) | **GET** /authentications/{id} | Show an existing Authentication
*TopologicalInventoryApiClient::DefaultApi* | [**show_container**](docs/DefaultApi.md#show_container) | **GET** /containers/{id} | Show an existing Container
*TopologicalInventoryApiClient::DefaultApi* | [**show_container_group**](docs/DefaultApi.md#show_container_group) | **GET** /container_groups/{id} | Show an existing ContainerGroup
*TopologicalInventoryApiClient::DefaultApi* | [**show_container_image**](docs/DefaultApi.md#show_container_image) | **GET** /container_images/{id} | Show an existing ContainerImage
*TopologicalInventoryApiClient::DefaultApi* | [**show_container_node**](docs/DefaultApi.md#show_container_node) | **GET** /container_nodes/{id} | Show an existing ContainerNode
*TopologicalInventoryApiClient::DefaultApi* | [**show_container_project**](docs/DefaultApi.md#show_container_project) | **GET** /container_projects/{id} | Show an existing ContainerProject
*TopologicalInventoryApiClient::DefaultApi* | [**show_container_template**](docs/DefaultApi.md#show_container_template) | **GET** /container_templates/{id} | Show an existing ContainerTemplate
*TopologicalInventoryApiClient::DefaultApi* | [**show_endpoint**](docs/DefaultApi.md#show_endpoint) | **GET** /endpoints/{id} | Show an existing Endpoint
*TopologicalInventoryApiClient::DefaultApi* | [**show_flavor**](docs/DefaultApi.md#show_flavor) | **GET** /flavors/{id} | Show an existing Flavor
*TopologicalInventoryApiClient::DefaultApi* | [**show_orchestration_stack**](docs/DefaultApi.md#show_orchestration_stack) | **GET** /orchestration_stacks/{id} | Show an existing OrchestrationStack
*TopologicalInventoryApiClient::DefaultApi* | [**show_service_instance**](docs/DefaultApi.md#show_service_instance) | **GET** /service_instances/{id} | Show an existing ServiceInstance
*TopologicalInventoryApiClient::DefaultApi* | [**show_service_offering**](docs/DefaultApi.md#show_service_offering) | **GET** /service_offerings/{id} | Show an existing ServiceOffering
*TopologicalInventoryApiClient::DefaultApi* | [**show_service_offering_icon**](docs/DefaultApi.md#show_service_offering_icon) | **GET** /service_offering_icons/{id} | Show an existing ServiceOfferingIcon
*TopologicalInventoryApiClient::DefaultApi* | [**show_service_plan**](docs/DefaultApi.md#show_service_plan) | **GET** /service_plans/{id} | Show an existing ServicePlan
*TopologicalInventoryApiClient::DefaultApi* | [**show_source**](docs/DefaultApi.md#show_source) | **GET** /sources/{id} | Show an existing Source
*TopologicalInventoryApiClient::DefaultApi* | [**show_source_type**](docs/DefaultApi.md#show_source_type) | **GET** /source_types/{id} | Show an existing SourceType
*TopologicalInventoryApiClient::DefaultApi* | [**show_tag**](docs/DefaultApi.md#show_tag) | **GET** /tags/{id} | Show an existing Tag
*TopologicalInventoryApiClient::DefaultApi* | [**show_task**](docs/DefaultApi.md#show_task) | **GET** /tasks/{id} | Show an existing Task
*TopologicalInventoryApiClient::DefaultApi* | [**show_vm**](docs/DefaultApi.md#show_vm) | **GET** /vms/{id} | Show an existing Vm
*TopologicalInventoryApiClient::DefaultApi* | [**show_volume**](docs/DefaultApi.md#show_volume) | **GET** /volumes/{id} | Show an existing Volume
*TopologicalInventoryApiClient::DefaultApi* | [**show_volume_attachment**](docs/DefaultApi.md#show_volume_attachment) | **GET** /volume_attachments/{id} | Show an existing VolumeAttachment
*TopologicalInventoryApiClient::DefaultApi* | [**show_volume_type**](docs/DefaultApi.md#show_volume_type) | **GET** /volume_types/{id} | Show an existing VolumeType
*TopologicalInventoryApiClient::DefaultApi* | [**update_authentication**](docs/DefaultApi.md#update_authentication) | **PATCH** /authentications/{id} | Update an existing Authentication
*TopologicalInventoryApiClient::DefaultApi* | [**update_endpoint**](docs/DefaultApi.md#update_endpoint) | **PATCH** /endpoints/{id} | Update an existing Endpoint
*TopologicalInventoryApiClient::DefaultApi* | [**update_source**](docs/DefaultApi.md#update_source) | **PATCH** /sources/{id} | Update an existing Source
*TopologicalInventoryApiClient::DefaultApi* | [**update_task**](docs/DefaultApi.md#update_task) | **PATCH** /tasks/{id} | Update an existing Task


## Documentation for Models

 - [TopologicalInventoryApiClient::Authentication](docs/Authentication.md)
 - [TopologicalInventoryApiClient::AuthenticationsCollection](docs/AuthenticationsCollection.md)
 - [TopologicalInventoryApiClient::CollectionLinks](docs/CollectionLinks.md)
 - [TopologicalInventoryApiClient::CollectionMetadata](docs/CollectionMetadata.md)
 - [TopologicalInventoryApiClient::Container](docs/Container.md)
 - [TopologicalInventoryApiClient::ContainerGroup](docs/ContainerGroup.md)
 - [TopologicalInventoryApiClient::ContainerGroupsCollection](docs/ContainerGroupsCollection.md)
 - [TopologicalInventoryApiClient::ContainerImage](docs/ContainerImage.md)
 - [TopologicalInventoryApiClient::ContainerImagesCollection](docs/ContainerImagesCollection.md)
 - [TopologicalInventoryApiClient::ContainerNode](docs/ContainerNode.md)
 - [TopologicalInventoryApiClient::ContainerNodesCollection](docs/ContainerNodesCollection.md)
 - [TopologicalInventoryApiClient::ContainerProject](docs/ContainerProject.md)
 - [TopologicalInventoryApiClient::ContainerProjectsCollection](docs/ContainerProjectsCollection.md)
 - [TopologicalInventoryApiClient::ContainerTemplate](docs/ContainerTemplate.md)
 - [TopologicalInventoryApiClient::ContainerTemplatesCollection](docs/ContainerTemplatesCollection.md)
 - [TopologicalInventoryApiClient::ContainersCollection](docs/ContainersCollection.md)
 - [TopologicalInventoryApiClient::Endpoint](docs/Endpoint.md)
 - [TopologicalInventoryApiClient::EndpointsCollection](docs/EndpointsCollection.md)
 - [TopologicalInventoryApiClient::Flavor](docs/Flavor.md)
 - [TopologicalInventoryApiClient::FlavorsCollection](docs/FlavorsCollection.md)
 - [TopologicalInventoryApiClient::IDReadOnly](docs/IDReadOnly.md)
 - [TopologicalInventoryApiClient::InlineResponse200](docs/InlineResponse200.md)
 - [TopologicalInventoryApiClient::OrchestrationStack](docs/OrchestrationStack.md)
 - [TopologicalInventoryApiClient::OrchestrationStacksCollection](docs/OrchestrationStacksCollection.md)
 - [TopologicalInventoryApiClient::OrderParameters](docs/OrderParameters.md)
 - [TopologicalInventoryApiClient::ServiceInstance](docs/ServiceInstance.md)
 - [TopologicalInventoryApiClient::ServiceInstancesCollection](docs/ServiceInstancesCollection.md)
 - [TopologicalInventoryApiClient::ServiceOffering](docs/ServiceOffering.md)
 - [TopologicalInventoryApiClient::ServiceOfferingIcon](docs/ServiceOfferingIcon.md)
 - [TopologicalInventoryApiClient::ServiceOfferingIconsCollection](docs/ServiceOfferingIconsCollection.md)
 - [TopologicalInventoryApiClient::ServiceOfferingsCollection](docs/ServiceOfferingsCollection.md)
 - [TopologicalInventoryApiClient::ServicePlan](docs/ServicePlan.md)
 - [TopologicalInventoryApiClient::ServicePlansCollection](docs/ServicePlansCollection.md)
 - [TopologicalInventoryApiClient::Source](docs/Source.md)
 - [TopologicalInventoryApiClient::SourceType](docs/SourceType.md)
 - [TopologicalInventoryApiClient::SourceTypesCollection](docs/SourceTypesCollection.md)
 - [TopologicalInventoryApiClient::SourcesCollection](docs/SourcesCollection.md)
 - [TopologicalInventoryApiClient::Tag](docs/Tag.md)
 - [TopologicalInventoryApiClient::Tagging](docs/Tagging.md)
 - [TopologicalInventoryApiClient::TagsCollection](docs/TagsCollection.md)
 - [TopologicalInventoryApiClient::Task](docs/Task.md)
 - [TopologicalInventoryApiClient::TasksCollection](docs/TasksCollection.md)
 - [TopologicalInventoryApiClient::Vm](docs/Vm.md)
 - [TopologicalInventoryApiClient::VmsCollection](docs/VmsCollection.md)
 - [TopologicalInventoryApiClient::Volume](docs/Volume.md)
 - [TopologicalInventoryApiClient::VolumeAttachment](docs/VolumeAttachment.md)
 - [TopologicalInventoryApiClient::VolumeAttachmentsCollection](docs/VolumeAttachmentsCollection.md)
 - [TopologicalInventoryApiClient::VolumeType](docs/VolumeType.md)
 - [TopologicalInventoryApiClient::VolumeTypesCollection](docs/VolumeTypesCollection.md)
 - [TopologicalInventoryApiClient::VolumesCollection](docs/VolumesCollection.md)


## Documentation for Authorization


### UserSecurity

- **Type**: HTTP basic authentication

