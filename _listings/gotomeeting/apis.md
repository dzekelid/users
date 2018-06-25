---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: SCIM Get User Schema
  x-api-slug: scim
  description: Queries the user schema. The user schema is defined in SCIM Core Schema
    (http://www.simplecloud.info/specs/draft-scim-core-schema-01.html#resource-schema).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Schemas/Users
  tags: Schemas,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/schemasusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/schemasusers-get-openapi.md
- name: SCIM Get Users
  x-api-slug: scim
  description: Queries multiple user identities in the organization domain. Filtering
    is available.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/users-get-openapi.md
- name: SCIM Create User
  x-api-slug: scim
  description: Creates a new organization user and adds them to the user domain. The
    user email domain must match an existing organization email domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/users-post-openapi.md
- name: SCIM Get Current User
  x-api-slug: scim
  description: Queries the identity of the current authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/me
  tags: Users,Me
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersme-get-openapi.md
- name: SCIM Update Current User
  x-api-slug: scim
  description: Changes a limited set (or all if you choose) of the current authenticated
    user's data. The updated user email domain must be an existing organization email
    domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/me
  tags: Users,Me
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersme-patch-openapi.md
- name: SCIM Replace Current User
  x-api-slug: scim
  description: Changes the current authenticated user's displayName, locale, timezone,
    username and password. The request must include the full user definition (to modify
    one or more values without sending the full definition, see Update User). The
    replaced user email domain must be an existing organization email domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/me
  tags: Users,Me
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersme-put-openapi.md
- name: SCIM Delete User
  x-api-slug: scim
  description: Deletes a user from the organization (but not from the account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/{userKey}
  tags: Users,UserKey
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersuserkey-delete-openapi.md
- name: SCIM Get User
  x-api-slug: scim
  description: Queries user identity in the organization domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/{userKey}
  tags: Users,UserKey
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersuserkey-get-openapi.md
- name: SCIM Update User
  x-api-slug: scim
  description: Changes a limited set (or all if you choose) of the user's data. The
    updated user email domain must be an existing organization email domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/{userKey}
  tags: Users,UserKey
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersuserkey-patch-openapi.md
- name: SCIM Replace User
  x-api-slug: scim
  description: Changes an existing user's displayName, locale, timezone, username
    and password. The request must include the full user definition (to modify one
    or more values without sending the full definition, see Update User). The replaced
    user email domain must be an existing organization email domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1//Users/{userKey}
  tags: Users,UserKey
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/usersuserkey-put-openapi.md
- name: SCIM
  x-api-slug: scim
  description: Citrix enables business mobility through the secure delivery of apps
    and data to any device on any network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gotomeeting/openapi.md
x-common:
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---