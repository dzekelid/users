---
swagger: "2.0"
x-collection-name: Product Hunt
x-complete: 1
info:
  title: Product Hunt
  description: the-api-for-product-hunt-
  version: 1.0.0
host: api.producthunt.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{username}:
    get:
      summary: Users
      description: Get Users
      operationId: users.username.get
      x-api-path-slug: usersusername-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Users
---