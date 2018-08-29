---
name: Spreaker
x-slug: spreaker
description: Discover and listen to your favorite podcasts for free or sign up to
  create your own!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/657-spreaker.jpg
x-kinRank: "8"
x-alexaRank: "12286"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/apis.md
specificationVersion: "0.14"
apis:
- name: Spreaker API Search users, shows and episodes
  x-api-slug: spreaker-api
  description: Search users, shows and episodes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/657-spreaker.jpg
  humanURL: http://spreaker.com
  baseURL: http://api.spreaker.com////search/{query}
  tags: Search,Users,,Shows,Episodes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/searchquery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/searchquery-get-openapi.md
- name: Spreaker API Search Users
  x-api-slug: spreaker-api
  description: This API allows to find users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/657-spreaker.jpg
  humanURL: http://spreaker.com
  baseURL: http://api.spreaker.com////users/search/{query}
  tags: Search,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/userssearchquery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/userssearchquery-get-openapi.md
- name: Spreaker API
  x-api-slug: spreaker-api
  description: Spreaker platform enables you to host and listen thousands of radio
    shows. Spreaker provides a REST web service that enables developers to read and
    write data to Spreaker.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/657-spreaker.jpg
  humanURL: http://spreaker.com
  baseURL: http://api.spreaker.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/spreaker/openapi.md
x-common:
- type: x-base
  url: http://api.spreaker.com/
- type: x-blog
  url: http://blog.spreaker.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/spreaker
- type: x-crunchbase
  url: http://www.crunchbase.com/company/spreaker
- type: x-developer
  url: http://developers.spreaker.com
- type: x-email
  url: info@spreaker.com
- type: x-email
  url: support@spreaker.com
- type: x-email
  url: advertise@spreaker.com
- type: x-email
  url: tonia.maffeo@spreaker.com
- type: x-email
  url: press@spreaker.com
- type: x-email
  url: legal@Spreaker.com
- type: x-github
  url: https://github.com/spreaker
- type: x-linkedin
  url: https://www.linkedin.com/company/spreaker/
- type: x-pricing
  url: http://www.spreaker.com/plans
- type: x-twitter
  url: https://twitter.com/spreaker
- type: x-website
  url: http://spreaker.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---