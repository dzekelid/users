---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users.{format}:
    get:
      summary: Get Users. Format
      description: |-
        Show a paginated list of all users.

        Uers can be filtered by their ids or email.
      operationId: getUsers.Format
      x-api-path-slug: users-format-get
      parameters:
      - in: query
        name: filter[email]
        description: Filter by user email
        type: string
      - in: query
        name: filter[ids]
        description: Filter by user IDs
        type: list
      - in: query
        name: page
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Users.
      - Format
  /users/{id}.{format}:
    get:
      summary: Get Users  . Format
      description: This API endpoint returns a single user, identified by ID.
      operationId: getUsers.Format
      x-api-path-slug: usersid-format-get
      parameters:
      - in: path
        name: id
        description: User ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - .
      - Format
  /users/{id}/reset_password.{format}:
    post:
      summary: Add Users  Reset Password. Format
      description: This API endpoints reset the user password, identified by ID
      operationId: postUsersResetPassword.Format
      x-api-path-slug: usersidreset-password-format-post
      parameters:
      - in: path
        name: id
        description: User ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Reset
      - Password.
      - Format
---