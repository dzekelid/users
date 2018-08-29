---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Users Username Following
  description: Parameters users username following
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
    parameters:
      summary: Parameters Users Username
      description: Parameters users username
      operationId: parametersUsersUsername
      x-api-path-slug: usersusername-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
  /users/{username}/followers:
    get:
      summary: Get Users Username Followers
      description: Returns the list of accounts that are following this team.
      operationId: getUsersUsernameFollowers
      x-api-path-slug: usersusernamefollowers-get
      parameters:
      - in: path
        name: username
        description: The accounts username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Followers
    parameters:
      summary: Parameters Users Username Followers
      description: Parameters users username followers
      operationId: parametersUsersUsernameFollowers
      x-api-path-slug: usersusernamefollowers-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Followers
  /users/{username}/following:
    get:
      summary: Get Users Username Following
      description: Returns the list of accounts this user is following.
      operationId: getUsersUsernameFollowing
      x-api-path-slug: usersusernamefollowing-get
      parameters:
      - in: path
        name: username
        description: The users username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Following
    parameters:
      summary: Parameters Users Username Following
      description: Parameters users username following
      operationId: parametersUsersUsernameFollowing
      x-api-path-slug: usersusernamefollowing-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Following
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