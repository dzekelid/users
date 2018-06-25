---
name: Azure API Management
x-slug: azure-api-management
description: Use Azure API Management as a turnkey solution for publishing APIs to
  external and internal customers. Quickly create consistent and modern API gateways
  for existing back-end services hosted anywhere, secure and protect them from abuse
  and overuse, and get insights into usage and health. Plus, automate and scale developer
  onboarding to help get your API program up and running.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/apis.md
specificationVersion: "0.14"
apis:
- name: Azure API Management API GroupUsers ListByGroups
  x-api-slug: azure-api-management-api
  description: Lists a collection of the members of the group, specified by its identifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users
  tags: Group Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusers-get-openapi.md
- name: Azure API Management API GroupUsers Create
  x-api-slug: azure-api-management-api
  description: Adds a user to the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users/{uid}
  tags: Group Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-put-openapi.md
- name: Azure API Management API GroupUsers Delete
  x-api-slug: azure-api-management-api
  description: Remove existing user from existing group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users/{uid}
  tags: Group Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-delete-openapi.md
- name: Azure API Management API Users ListByService
  x-api-slug: azure-api-management-api
  description: Lists a collection of registered users in the specified service instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusers-get-openapi.md
- name: Azure API Management API Users Get
  x-api-slug: azure-api-management-api
  description: Gets the details of the user specified by its identifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-get-openapi.md
- name: Azure API Management API Users CreateOrUpdate
  x-api-slug: azure-api-management-api
  description: Creates or Updates a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-put-openapi.md
- name: Azure API Management API Users Update
  x-api-slug: azure-api-management-api
  description: Updates the details of the user specified by its identifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-patch-openapi.md
- name: Azure API Management API Users Delete
  x-api-slug: azure-api-management-api
  description: Deletes specific user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-delete-openapi.md
- name: Azure API Management API Users GenerateSsoUrl
  x-api-slug: azure-api-management-api
  description: Retrieves a redirection URL containing an authentication token for
    signing a given user into the developer portal.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/generateSsoUrl
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgeneratessourl-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgeneratessourl-post-openapi.md
- name: Azure API Management API UserGroups ListByUsers
  x-api-slug: azure-api-management-api
  description: Lists all user groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/groups
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgroups-get-openapi.md
- name: Azure API Management API UserSubscriptions ListByUsers
  x-api-slug: azure-api-management-api
  description: Lists the collection of subscriptions of the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/subscriptions
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidsubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidsubscriptions-get-openapi.md
- name: Azure API Management API UserIdentities ListByUsers
  x-api-slug: azure-api-management-api
  description: Lists all user identities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/identities
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuididentities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuididentities-get-openapi.md
- name: Azure API Management API
  x-api-slug: azure-api-management-api
  description: Use Azure API Management as a turnkey solution for publishing APIs
    to external and internal customers. Quickly create consistent and modern API gateways
    for existing back-end services hosted anywhere, secure and protect them from abuse
    and overuse, and get insights into usage and health. Plus, automate and scale
    developer onboarding to help get your API program up and running.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-api-management/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/api-management/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/api-management/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/api-management/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/api-management/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---