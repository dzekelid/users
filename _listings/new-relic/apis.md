---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Users. Format
  x-api-slug: new-relic
  description: |-
    Show a paginated list of all users.

    Uers can be filtered by their ids or email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users.{format}
  tags: Users., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/new-relic/users-format-get-openapi.md
- name: New Relic Get Users  . Format
  x-api-slug: new-relic
  description: This API endpoint returns a single user, identified by ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users/{id}.{format}
  tags: Users, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/new-relic/usersid-format-get-openapi.md
- name: New Relic Add Users  Reset Password. Format
  x-api-slug: new-relic
  description: This API endpoints reset the user password, identified by ID
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users/{id}/reset_password.{format}
  tags: Users, , Reset, Password., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/new-relic/usersidreset-password-format-post-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic???s digital intelligence platform lets developers, ops, and
    tech teams measure and monitor the performance of their applications and infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---