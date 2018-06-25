---
name: Gitter
x-slug: gitter
description: Gitter is a chat and networking platform that helps to manage, grow and
  connect communities through messaging, content and discovery.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
x-kinRank: "8"
x-alexaRank: "18282"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/apis.md
specificationVersion: "0.14"
apis:
- name: Gitter API Room Users
  x-api-slug: gitter-api
  description: List of Users currently in the room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/users
  tags: Rooms,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/roomsroomidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/roomsroomidusers-get-openapi.md
- name: Gitter API Get User
  x-api-slug: gitter-api
  description: Get the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/user-get-openapi.md
- name: Gitter API Get User Rooms
  x-api-slug: gitter-api
  description: List of Rooms the user is part of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms
  tags: Users,Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridrooms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridrooms-get-openapi.md
- name: Gitter API Get User Unread Items
  x-api-slug: gitter-api
  description: You can retrieve unread items and mentions using the following endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms/:roomId/unreadItems
  tags: Users,Messages,Unread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridroomsroomidunreaditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridroomsroomidunreaditems-get-openapi.md
- name: Gitter API User Orgs
  x-api-slug: gitter-api
  description: List of the user's GitHub Organisations and their respective Room if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/orgs
  tags: Users,Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridorgs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridorgs-get-openapi.md
- name: Gitter API User Repos
  x-api-slug: gitter-api
  description: List of the user's GitHub Repositories and their respective Room if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/repos
  tags: Users,Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridrepos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridrepos-get-openapi.md
- name: Gitter API Get User Channels
  x-api-slug: gitter-api
  description: List of Gitter channels nested under the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/channels
  tags: Users,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridchannels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/useruseridchannels-get-openapi.md
- name: Gitter API
  x-api-slug: gitter-api
  description: Gitter is a chat and networking platform that helps to manage, grow
    and connect communities through messaging, content and discovery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https:///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/gitter/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/gitter
- type: x-developer
  url: https://developer.gitter.im/docs/streaming-api
- type: x-github
  url: https://github.com/gitterHQ
- type: x-curated-source
  url: https://gitter.im/apiaryio/api-blueprint
- type: x-website
  url: http://gitter.im
- type: x-twitter
  url: https://twitter.com/gitchat
- type: x-website
  url: https://gitter.im
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---