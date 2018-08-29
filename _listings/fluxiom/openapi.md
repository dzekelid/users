---
swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 1
info:
  title: Fluxiom API
  description: the-fluxiom-api-allows-you-to-hook-into-fluxiom-and-connect-it-with-other-apps-
  termsOfService: http://www.fluxiom.com/terms
  version: v1
host: '{subdomain}.fluxiom.com'
basePath: /api/{format}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/users:
    get:
      summary: Get users
      description: Get users
      operationId: get-users
      x-api-path-slug: apiusers-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /api/users/{id}:
    get:
      summary: Get single user
      description: Get single user
      operationId: get-single-user
      x-api-path-slug: apiusersid-get
      parameters:
      - in: path
        name: id
        description: Unique id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
---