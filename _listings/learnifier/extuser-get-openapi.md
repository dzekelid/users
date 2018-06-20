---
swagger: "2.0"
x-collection-name: Learnifier
x-complete: 0
info:
  title: Learnifier Gets a user by external id
  version: 1.1.0
  description: Gets a user by external id.
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extuser:
    get:
      summary: Gets a user by external id
      description: Gets a user by external id.
      operationId: extuser.get
      x-api-path-slug: extuser-get
      parameters:
      - in: query
        name: extid
        description: The external id of the user
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