---
name: PagerDuty
x-slug: pagerduty
description: See how PagerDuty Digital Operations Management Platform integrates machine
  data & human intelligence to improve visibility & agility across organizations.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
x-kinRank: "8"
x-alexaRank: "19574"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/apis.md
specificationVersion: "0.14"
apis:
- name: PagerDuty Users {user_guid}
  x-api-slug: pagerduty
  description: Returns customer's user by user GUID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: 'https://///users/{user_guid} '
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersuser-guid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersuser-guid-get-openapi.md
- name: PagerDuty Users
  x-api-slug: pagerduty
  description: Returns all customer's users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: 'https://///users '
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-get-openapi.md
- name: PagerDuty Users
  x-api-slug: pagerduty
  description: Creates a new user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: 'https://///users '
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-post-openapi.md
- name: PagerDuty Users
  x-api-slug: pagerduty
  description: Updates a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: 'https://///users '
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-put-openapi.md
- name: PagerDuty Users {user_guid}
  x-api-slug: pagerduty
  description: DELETE users user gu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: 'https://///users/{user_guid} '
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersuser-guid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersuser-guid-delete-openapi.md
- name: PagerDuty Remove a user from a team
  x-api-slug: pagerduty
  description: Remove a user from a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///teams/{id}/users/{user_id}
  tags: Team Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/teamsidusersuser-id-delete-openapi.md
- name: PagerDuty Add a user to a team
  x-api-slug: pagerduty
  description: Add a user to a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///teams/{id}/users/{user_id}
  tags: Team Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/teamsidusersuser-id-put-openapi.md
- name: PagerDuty List users
  x-api-slug: pagerduty
  description: List users of your PagerDuty account, optionally filtered by a search
    query.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-get-openapi.md
- name: PagerDuty Create a user
  x-api-slug: pagerduty
  description: Create a new user. Note that you must also supply a `password` property
    to create a user--it will not be returned by any API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/users-post-openapi.md
- name: PagerDuty Get a user
  x-api-slug: pagerduty
  description: Get details about an existing user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users/{id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersid-get-openapi.md
- name: PagerDuty Delete a user
  x-api-slug: pagerduty
  description: Remove an existing user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users/{id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersid-delete-openapi.md
- name: PagerDuty Update a user
  x-api-slug: pagerduty
  description: Update an existing user. Note that you may also supply a `password`
    property--it will not be returned by any API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users/{id}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersid-put-openapi.md
- name: PagerDuty Deleting a user
  x-api-slug: pagerduty
  description: users users user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https://///users/users/userId
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/usersusersuserid--openapi.md
- name: PagerDuty
  x-api-slug: pagerduty
  description: See how PagerDuty Digital Operations Management Platform integrates
    machine data & human intelligence to improve visibility & agility across organizations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com
  baseURL: https:///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/pagerduty/openapi.md
x-common:
- type: x-base
  url: https://acme.pagerduty.com/api/
- type: x-blog
  url: http://blog.pagerduty.com/
- type: x-blog-rss
  url: http://blog.pagerduty.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/pagerduty
- type: x-crunchbase
  url: https://crunchbase.com/organization/pagerduty
- type: x-developer
  url: http://developer.pagerduty.com/
- type: x-email
  url: info@pagerduty.com
- type: x-email
  url: sales@pagerduty.com
- type: x-email
  url: support@pagerduty.com
- type: x-email
  url: legal@pagerduty.com
- type: x-github
  url: https://github.com/PagerDuty
- type: x-openapi-spec--authoritative
  url: https://api-reference.pagerduty.com/output.json
- type: x-pricing
  url: https://www.pagerduty.com/pricing/
- type: x-twitter
  url: https://twitter.com/pagerduty
- type: x-website
  url: http://www.pagerduty.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---