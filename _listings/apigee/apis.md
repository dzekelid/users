---
name: Apigee
x-slug: apigee
description: Apigee Edge is a platform for developing and managing API proxies. Think
  of a proxy as an abstraction layer that fronts for your backend service APIs and
  provides value-added features like security, rate limiting, quotas, analytics, and
  more. The primary consumers of Edge API proxies are app developers who want to use
  your backend services.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/apis.md
specificationVersion: "0.14"
apis:
- name: Apigee Edge Get Users
  x-api-slug: apigee-edge
  description: Gets a list of users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/users-get-openapi.md
- name: Apigee Edge Post Users
  x-api-slug: apigee-edge
  description: Creates a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/users-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/users-post-openapi.md
- name: Apigee Edge Get Users User Email
  x-api-slug: apigee-edge
  description: Gets a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-get-openapi.md
- name: Apigee Edge Post Users User Email
  x-api-slug: apigee-edge
  description: Updates a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-post-openapi.md
- name: Apigee Edge Delete Users User Email
  x-api-slug: apigee-edge
  description: Deletes a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-email-delete-openapi.md
- name: Apigee Edge Get Users User Email Userroles
  x-api-slug: apigee-edge
  description: Gets roles for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles
  tags: Users,User,Email,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserroles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserroles-get-openapi.md
- name: Apigee Edge Post Users User Email Userroles
  x-api-slug: apigee-edge
  description: Associates a user with a organizational user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles
  tags: Users,User,Email,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserroles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserroles-post-openapi.md
- name: Apigee Edge Get Userroles Role Name Users
  x-api-slug: apigee-edge
  description: Lists users for a role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users
  tags: Userroles,Role,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusers-get-openapi.md
- name: Apigee Edge Post Userroles Role Name Users
  x-api-slug: apigee-edge
  description: Adds user to role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users
  tags: Userroles,Role,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusers-post-openapi.md
- name: Apigee Edge Get Userroles Role Name Users User Email
  x-api-slug: apigee-edge
  description: Checks user in a given system role
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users/{user_email}
  tags: Userroles,Role,Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusersuser-email-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusersuser-email-get-openapi.md
- name: Apigee Edge Delete Userroles Role Name Users User Email
  x-api-slug: apigee-edge
  description: Deletes user for a role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users/{user_email}
  tags: Userroles,Role,Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusersuser-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/userrolesrole-nameusersuser-email-delete-openapi.md
- name: Apigee Edge Delete Users User Email Userroles Role Name
  x-api-slug: apigee-edge
  description: Deletes organizational role for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles/{role_name}
  tags: Users,User,Email,Userroles,Role
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserrolesrole-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailuserrolesrole-name-delete-openapi.md
- name: Apigee Edge Get Users User Name Permissions
  x-api-slug: apigee-edge
  description: Gets permissions for a user at global level
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_name}/permissions
  tags: Users,User,Permissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-namepermissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-namepermissions-get-openapi.md
- name: Apigee Edge Get Users User Email Permissions Get
  x-api-slug: apigee-edge
  description: Checks user has particular permission for a resource at global level
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}permissions/get
  tags: Users,User,Emailpermissions,Get
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailpermissionsget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/usersuser-emailpermissionsget-get-openapi.md
- name: Apigee Edge
  x-api-slug: apigee-edge
  description: Apigee Edge is a platform for developing and managing API proxies.
    Think of a proxy as an abstraction layer that fronts for your backend service
    APIs and provides value-added features like security, rate limiting, quotas, analytics,
    and more. The primary consumers of Edge API proxies are app developers who want
    to use your backend services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/apigee/openapi.md
x-common:
- type: x-website
  url: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---