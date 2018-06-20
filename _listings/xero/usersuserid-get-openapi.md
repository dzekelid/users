---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Users User
  description: Get users user.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Users:
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
    x-related-model:
      summary: X-related-model Users
      description: X-related-model users.
      operationId: x-related-modelUsers
      x-api-path-slug: users-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Users
  /Users/{UserID}:
    get:
      summary: Get Users User
      description: Get users user.
      operationId: getUsersUser
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: UserID
      responses:
        200:
          description: OK
      tags:
      - Users
      - UserID
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