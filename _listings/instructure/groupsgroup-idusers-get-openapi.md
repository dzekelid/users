---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API List groups users
  description: List groups users.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/users:
    get:
      summary: List groups users
      description: List groups users.
      operationId: list-groups-users
      x-api-path-slug: groupsgroup-idusers-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cavatar_urlu201d: Include users&#39; avatar_urls'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
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