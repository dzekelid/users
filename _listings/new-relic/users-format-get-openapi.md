---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Users. Format
  version: 1.0.0
  description: |-
    Show a paginated list of all users.

    Uers can be filtered by their ids or email.
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