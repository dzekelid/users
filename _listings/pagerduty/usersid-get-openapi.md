---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Get a user
  version: 1.0.0
  description: Get details about an existing user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/users/{user_guid} ':
    ' get ':
      summary: Users {user_guid}
      description: Returns customer's user by user GUID.
      operationId: ""
      x-api-path-slug: usersuser-guid-get
      responses:
        200:
          description: OK
      tags:
      - Users
    ' delete ':
      summary: Users {user_guid}
      description: DELETE users user gu
      operationId: ""
      x-api-path-slug: usersuser-guid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
  '/users ':
    ' get ':
      summary: Users
      description: Returns all customer's users.
      operationId: ""
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    ' post ':
      summary: Users
      description: Creates a new user.
      operationId: ""
      x-api-path-slug: users-post
      responses:
        200:
          description: OK
      tags:
      - Users
    ' put ':
      summary: Users
      description: Updates a user.
      operationId: ""
      x-api-path-slug: users-put
      responses:
        200:
          description: OK
      tags:
      - Users
  /teams/{id}/users/{user_id}:
    delete:
      summary: Remove a user from a team
      description: Remove a user from a team.
      operationId: remove-a-user-from-a-team
      x-api-path-slug: teamsidusersuser-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team Users
    put:
      summary: Add a user to a team
      description: Add a user to a team.
      operationId: add-a-user-to-a-team
      x-api-path-slug: teamsidusersuser-id-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team Users
  /users:
    get:
      summary: List users
      description: List users of your PagerDuty account, optionally filtered by a
        search query.
      operationId: list-users-of-your-pagerduty-account-optionally-filtered-by-a-search-query
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: query
        description: Filters the result, showing only the users whose names or email
          addresses match the query
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Create a user
      description: Create a new user. Note that you must also supply a `password`
        property to create a user--it will not be returned by any API.
      operationId: create-a-new-user-note-that-you-must-also-supply-a-password-property-to-create-a-userit-will-not-be-
      x-api-path-slug: users-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: user
        description: The user to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{id}:
    get:
      summary: Get a user
      description: Get details about an existing user.
      operationId: get-details-about-an-existing-user
      x-api-path-slug: usersid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
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