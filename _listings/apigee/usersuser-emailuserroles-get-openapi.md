---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Get Users User Email Userroles
  description: Gets roles for a user.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get Users
      description: Gets a list of users.
      operationId: getUsers
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: Creates a user.
      operationId: postUsers
      x-api-path-slug: users-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_email}:
    get:
      summary: Get Users User Email
      description: Gets a user.
      operationId: getUsersUserEmail
      x-api-path-slug: usersuser-email-get
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
    post:
      summary: Post Users User Email
      description: Updates a user.
      operationId: postUsersUserEmail
      x-api-path-slug: usersuser-email-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
    delete:
      summary: Delete Users User Email
      description: Deletes a user.
      operationId: deleteUsersUserEmail
      x-api-path-slug: usersuser-email-delete
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
  /users/{user_email}/userroles:
    get:
      summary: Get Users User Email Userroles
      description: Gets roles for a user.
      operationId: getUsersUserEmailUserroles
      x-api-path-slug: usersuser-emailuserroles-get
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
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