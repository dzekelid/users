---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 1
info:
  title: User API
  description: the-user-api-
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}:
    get:
      summary: Retrieve an user info
      description: Retrieve information for an existing user.
      operationId: retrieve-an-user-info
      x-api-path-slug: usersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
    delete:
      summary: Delete an user
      description: Delete an existing User.
      operationId: delete-an-user
      x-api-path-slug: usersuser-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
---