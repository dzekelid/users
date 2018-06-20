---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Get Users Username
  description: |-
    Gets the public information associated with a user account.

    If the user's profile is private, `location`, `website` and
    `created_on` elements are omitted.
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{username}:
    get:
      summary: Get Users Username
      description: |-
        Gets the public information associated with a user account.

        If the user's profile is private, `location`, `website` and
        `created_on` elements are omitted.
      operationId: getUsersUsername
      x-api-path-slug: usersusername-get
      parameters:
      - in: path
        name: username
        description: The accounts username or UUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---