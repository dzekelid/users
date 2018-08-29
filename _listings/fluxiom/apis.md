---
name: Fluxiom
x-slug: fluxiom
description: Fluxiom offers seamless online file management in the cloud. Keep your
  files private, share them with a select audience or broadcast them to the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/594-fluxiom.jpg
x-kinRank: "7"
x-alexaRank: "3532345"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/apis.md
specificationVersion: "0.14"
apis:
- name: Fluxiom API Get users
  x-api-slug: fluxiom-api
  description: Get users
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/594-fluxiom.jpg
  humanURL: http://fluxiom.com
  baseURL: https://{subdomain}.fluxiom.com//api/{format}//api/users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/apiusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/apiusers-get-openapi.md
- name: Fluxiom API Get single user
  x-api-slug: fluxiom-api
  description: Get single user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/594-fluxiom.jpg
  humanURL: http://fluxiom.com
  baseURL: https://{subdomain}.fluxiom.com//api/{format}//api/users/{id}
  tags: Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/apiusersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/apiusersid-get-openapi.md
- name: Fluxiom API
  x-api-slug: fluxiom-api
  description: The Fluxiom API allows you to hook into Fluxiom and connect it with
    other apps.  It can be used for retrieving and uploading assets, querying metadata,
    and more.  This enables Fluxiom to easily integrate with your workflow and the
    tools you already use.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/594-fluxiom.jpg
  humanURL: http://fluxiom.com
  baseURL: https://{subdomain}.fluxiom.com//api/{format}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/fluxiom/openapi.md
x-common:
- type: x-base
  url: https://fluxiom.com/api/
- type: x-blog
  url: http://blog.fluxiom.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/fluxiom
- type: x-crunchbase
  url: https://crunchbase.com/organization/product/fluxiom/timeline
- type: x-developer
  url: http://www.fluxiom.com/api
- type: x-email
  url: support@fluxiom.com
- type: x-privacy
  url: http://www.fluxiom.com/privacy
- type: x-terms-of-service
  url: http://www.fluxiom.com/terms
- type: x-twitter
  url: https://twitter.com/fluxiom
- type: x-website
  url: http://fluxiom.com
- type: x-website
  url: http://www.fluxiom.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---