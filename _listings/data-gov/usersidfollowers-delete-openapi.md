---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Delete Users  Followers
  description: Unfollow an object given its ID
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/:
    get:
      summary: Get Users
      description: List all objects
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: organization
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Add Users
      description: Create a new object
      operationId: postUsers
      x-api-path-slug: users-post
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/suggest/:
    get:
      summary: Get Users Suggest
      description: Suggest users
      operationId: getUsersSuggest
      x-api-path-slug: userssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggest
  /users/{id}/followers/:
    delete:
      summary: Delete Users  Followers
      description: Unfollow an object given its ID
      operationId: deleteUsersFollowers
      x-api-path-slug: usersidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
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