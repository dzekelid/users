---
swagger: "2.0"
x-collection-name: Product Hunt
x-complete: 0
info:
  title: Product Hunt Users
  description: Get Users
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