---
name: Medium
x-slug: medium
description: Medium is an online publishing platform founded by Twitter co-founder
  Evan Williams in August 2012. The platform has evolved into a hybrid of non-professional
  contributions and professional, paid contributions, an example of social journalism.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/medium/apis.md
specificationVersion: "0.14"
apis:
- name: Medium Create User Post
  x-api-slug: medium
  description: "Creates a post on the authenticated user\u2019s profile."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//users/{authorId}/posts
  tags: Users, Author, Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/medium/usersauthoridposts-post-openapi.md
- name: Medium User's publications
  x-api-slug: medium
  description: Returns a full list of publications that the user is related to in
    some way. This includes all publications the user is subscribed to, writes to,
    or edits.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//users/{userId}/publications
  tags: Users, User, Publications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/medium/usersuseridpublications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/medium/usersuseridpublications-get-openapi.md
- name: Medium
  x-api-slug: medium
  description: Medium is an online publishing platform founded by Twitter co-founder
    Evan Williams in August 2012. The platform has evolved into a hybrid of non-professional
    contributions and professional, paid contributions, an example of social journalism.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/medium/openapi.md
x-common:
- type: x-github
  url: https://github.com/Medium
- type: x-transparency-report
  url: https://medium.com/transparency-report
- type: x-twitter
  url: https://twitter.com/Medium
- type: x-website
  url: https://medium.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---