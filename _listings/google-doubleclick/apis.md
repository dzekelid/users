---
name: Google Doubleclick
x-slug: google-doubleclick
description: The Ad Exchange Buyer REST API allows your Real-Time Bidding application
  to access and update account information and to submit creatives. The API also allows
  an application (whether it does static bidding or real-time bidding) to discover
  direct deals that sellers make available.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/apis.md
specificationVersion: "0.14"
apis:
- name: Google Doubleclick API Get User Role Permission Groups
  x-api-slug: google-doubleclick-api
  description: Gets a list of all supported user role permission groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRolePermissionGroups
  tags: Advertising,Users, Roles, Permissions Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolepermissiongroups-get-openapi.md
- name: Google Doubleclick API Get User Role Permission Group
  x-api-slug: google-doubleclick-api
  description: Gets one user role permission group by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRolePermissionGroups/{id}
  tags: Advertising,Users, Roles, Permissions Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolepermissiongroupsid-get-openapi.md
- name: Google Doubleclick API Get User Role Permissions
  x-api-slug: google-doubleclick-api
  description: Gets a list of user role permissions, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRolePermissions
  tags: Advertising,Users, Roles, Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolepermissions-get-openapi.md
- name: Google Doubleclick API Get User Role Permission
  x-api-slug: google-doubleclick-api
  description: Gets one user role permission by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRolePermissions/{id}
  tags: Advertising,Users, Roles, Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolepermissionsid-get-openapi.md
- name: Google Doubleclick API Get User Roles
  x-api-slug: google-doubleclick-api
  description: Retrieves a list of user roles, possibly filtered. This method supports
    paging.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserroles-get-openapi.md
- name: Google Doubleclick API Update User Role
  x-api-slug: google-doubleclick-api
  description: Updates an existing user role. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserroles-patch-openapi.md
- name: Google Doubleclick API Insert User Role
  x-api-slug: google-doubleclick-api
  description: Inserts a new user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserroles-post-openapi.md
- name: Google Doubleclick API Update User Role
  x-api-slug: google-doubleclick-api
  description: Updates an existing user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserroles-put-openapi.md
- name: Google Doubleclick API Delete User Role
  x-api-slug: google-doubleclick-api
  description: Deletes an existing user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles/{id}
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolesid-delete-openapi.md
- name: Google Doubleclick API Get User Role
  x-api-slug: google-doubleclick-api
  description: Gets one user role by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https://///userprofiles/{profileId}/userRoles/{id}
  tags: Advertising,Users, Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/userprofilesprofileiduserrolesid-get-openapi.md
- name: Google Doubleclick API
  x-api-slug: google-doubleclick-api
  description: The Ad Exchange Buyer REST API allows your Real-Time Bidding application
    to access and update account information and to submit creatives. The API also
    allows an application (whether it does static bidding or real-time bidding) to
    discover direct deals that sellers make available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-double-click.png
  humanURL: https://www.doubleclickbygoogle.com/
  baseURL: https:///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-doubleclick/openapi.md
x-common:
- type: x-authentication
  url: https://developers.google.com/ad-exchange/buyer-rest/auth-guide
- type: x-blog
  url: http://googleadsdeveloper.blogspot.com/search/label/ad_exchange
- type: x-blog-rss
  url: http://googleadsdeveloper.blogspot.com/feeds/posts/default?alt=rss
- type: x-developer
  url: https://developers.google.com/ad-exchange/buyer-rest/
- type: x-forum
  url: https://groups.google.com/forum/#!forum/google-doubleclick-ad-exchange-buyer-api
- type: x-getting-started
  url: https://developers.google.com/ad-exchange/buyer-rest/start
- type: x-support
  url: https://developers.google.com/ad-exchange/buyer-rest/community/
- type: x-website
  url: https://www.doubleclickbygoogle.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---