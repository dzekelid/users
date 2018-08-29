---
swagger: "2.0"
x-collection-name: Medium
x-complete: 0
info:
  title: Medium User's publications
  description: Returns a full list of publications that the user is related to in
    some way. This includes all publications the user is subscribed to, writes to,
    or edits.
  termsOfService: https://medium.com/@feerst/2b405a832a2f
  contact:
    name: Hossain Khan
    url: https://github.com/amardeshbd/medium-api-specification
  version: 1.0.0
host: api.medium.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{authorId}/posts:
    post:
      summary: Create User Post
      description: "Creates a post on the authenticated user\u2019s profile."
      operationId: users.authorId.posts.post
      x-api-path-slug: usersauthoridposts-post
      parameters:
      - in: path
        name: authorId
        description: authorId is the user id of the authenticated user
      - in: body
        name: body
        description: Creates a post for user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Author
      - Posts
  /users/{userId}/publications:
    get:
      summary: User's publications
      description: Returns a full list of publications that the user is related to
        in some way. This includes all publications the user is subscribed to, writes
        to, or edits.
      operationId: users.userId.publications.get
      x-api-path-slug: usersuseridpublications-get
      parameters:
      - in: path
        name: userId
        description: A unique identifier for the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Publications
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