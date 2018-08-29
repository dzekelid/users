---
name: Venmo
x-slug: venmo
description: Venmo is a free digital wallet that lets you make and share payments
  with friends. You can easily split the bill, cab fare, or much more. Download the
  iOS or Android app or sign up on Venmo.com today.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2177-venmo.jpg
x-kinRank: "8"
x-alexaRank: "3421"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/apis.md
specificationVersion: "0.14"
apis:
- name: Venmo API Get Users User
  x-api-slug: venmo-api
  description: Get users user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2177-venmo.jpg
  humanURL: https://venmo.com/
  baseURL: https://api.venmo.com//v1//users/{user_id}
  tags: Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/usersuser-id-get-openapi.md
- name: Venmo API Get Users User Friends
  x-api-slug: venmo-api
  description: Get users user friends.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2177-venmo.jpg
  humanURL: https://venmo.com/
  baseURL: https://api.venmo.com//v1//users/{user_id}/friends
  tags: Users,User,Id,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/usersuser-idfriends-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/usersuser-idfriends-get-openapi.md
- name: Venmo API
  x-api-slug: venmo-api
  description: The Venmo API provides developers a straightforward way to integrate
    Venmo into their applications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2177-venmo.jpg
  humanURL: https://venmo.com/
  baseURL: https://api.venmo.com//v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/venmo/openapi.md
x-common:
- type: x-android-sdk
  url: https://github.com/venmo/app-switch-android
- type: x-authentication
  url: https://developer.venmo.com/docs/authentication
- type: x-blog
  url: http://blog.venmo.com/
- type: x-blog-rss
  url: http://blog.venmo.com/rss
- type: x-branding
  url: http://brand.venmo.com/styleguide
- type: x-buttons
  url: https://developer.venmo.com/docs/widgets/venmo-button
- type: x-console
  url: https://developer.venmo.com/docs/api-console
- type: x-crunchbase
  url: http://www.crunchbase.com/company/venmo
- type: x-crunchbase
  url: https://crunchbase.com/organization/venmo
- type: x-developer
  url: https://developer.venmo.com/
- type: x-email
  url: press@venmo.com
- type: x-email
  url: cardsupport@venmo.com
- type: x-email
  url: venmo@venmo.com
- type: x-email
  url: Support@venmo.com
- type: x-email
  url: privacy@venmo.com
- type: x-email
  url: legal+useragreement@venmo.com
- type: x-error-codes
  url: https://developer.venmo.com/docs/errors
- type: x-faq
  url: https://developer.venmo.com/docs/faq
- type: x-getting-started
  url: https://developer.venmo.com/docs/quickstart
- type: x-github
  url: https://github.com/venmo
- type: x-ios-sdk
  url: https://github.com/venmo/venmo-ios-sdk
- type: x-sandbox-environment
  url: https://developer.venmo.com/docs/sandbox
- type: x-twitter
  url: https://twitter.com/venmo
- type: x-webhooks
  url: https://developer.venmo.com/docs/webhooks
- type: x-website
  url: https://venmo.com/
- type: x-website
  url: http://venmo.com
- type: x-widgets
  url: https://developer.venmo.com/docs/widgets/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---