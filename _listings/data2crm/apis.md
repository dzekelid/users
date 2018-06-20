---
name: Data2CRM
x-slug: data2crm
description: Data2CRM is all-in-one master touch instrument to create the perfect
  data environment for prosperous internal and external connections.Data2CRM.API,
  a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/apis.md
specificationVersion: "0.14"
apis:
- name: Data2CRM GET for User
  x-api-slug: data2crm
  description: Returns all users from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/user-get-openapi.md
- name: Data2CRM POST for User
  x-api-slug: data2crm
  description: Add user into the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/user-post-openapi.md
- name: Data2CRM COUNT for User
  x-api-slug: data2crm
  description: Count all users from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user/count
  tags: Users,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/usercount-get-openapi.md
- name: Data2CRM DESCRIBE for User
  x-api-slug: data2crm
  description: Returns describe for users
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user/describe
  tags: Users,Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/userdescribe-get-openapi.md
- name: Data2CRM DELETE for User
  x-api-slug: data2crm
  description: Delete user information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user/{user_id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/useruser-id-delete-openapi.md
- name: Data2CRM GET for User
  x-api-slug: data2crm
  description: Return user information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user/{user_id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/useruser-id-get-openapi.md
- name: Data2CRM PUT for User
  x-api-slug: data2crm
  description: Update user information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//user/{user_id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/useruser-id-put-openapi.md
- name: Data2CRM
  x-api-slug: data2crm
  description: Data2CRM is all-in-one master touch instrument to create the perfect
    data environment for prosperous internal and external connections.Data2CRM.API,
    a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/data2crm/openapi.md
x-common:
- type: x-twitter
  url: https://twitter.com/data2crm
- type: x-website
  url: http://data2crm.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---