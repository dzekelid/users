---
swagger: "2.0"
x-collection-name: Zendesk
x-complete: 1
info:
  title: Sales Force Desk API
  description: build-deep-integrations-expose-your-service-to-influential-smb-customers-or-just-make-desk-com-work-the-way-you-want-
  version: v2
host: yoursite.desk.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users.{format}:
    get:
      summary: Get Users
      description: Get users.
      operationId: get-users
      x-api-path-slug: users-format-get
      parameters:
      - in: path
        name: format
      responses:
        200:
          description: OK
      tags:
      - Users
      - Format
  /users/{id}.{format}:
    get:
      summary: Get User
      description: Get user.
      operationId: get-user
      x-api-path-slug: usersid-format-get
      parameters:
      - in: path
        name: format
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Format
---