---
name: Azure DevTest Labs
x-slug: azure-devtest-labs
description: Azure DevTest Labs makes it easy to quickly create environments to deploy
  and test applications. Use reusable templates and artifacts to build Windows and
  Linux environments while minimalizing waste and controlling costs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/apis.md
specificationVersion: "0.14"
apis:
- name: Azure DevTest Labs API Users List
  x-api-slug: azure-devtest-labs-api
  description: List user profiles in a given lab.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusers-get-openapi.md
- name: Azure DevTest Labs API Users Get
  x-api-slug: azure-devtest-labs-api
  description: Get user profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/users/{name}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-get-openapi.md
- name: Azure DevTest Labs API Users Create Or Update
  x-api-slug: azure-devtest-labs-api
  description: Create or replace an existing user profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/users/{name}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-put-openapi.md
- name: Azure DevTest Labs API Users Delete
  x-api-slug: azure-devtest-labs-api
  description: Delete user profile. This operation can take a while to complete.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/users/{name}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-delete-openapi.md
- name: Azure DevTest Labs API Users Update
  x-api-slug: azure-devtest-labs-api
  description: Modify properties of user profiles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/users/{name}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameusersname-patch-openapi.md
- name: Azure DevTest Labs API
  x-api-slug: azure-devtest-labs-api
  description: Azure DevTest Labs makes it easy to quickly create environments to
    deploy and test applications. Use reusable templates and artifacts to build Windows
    and Linux environments while minimalizing waste and controlling costs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/azure-devtest-labs/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/devtest-lab/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/devtest-lab/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/devtest-lab/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/devtest-lab/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---