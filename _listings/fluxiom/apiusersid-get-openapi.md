---
swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 0
info:
  title: Fluxiom API Get single user
  description: Get single user
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