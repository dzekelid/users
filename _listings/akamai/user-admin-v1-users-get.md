---
swagger: "2.0"
info:
  title: Akamai API List a Group&#8217;s Users
  description: List a Group&#8217;s Users
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user-admin/v1/users:
    get:
      summary: List a Group&#8217;s Users
      description: List a Group&#8217;s Users
      operationId: useradminv1usersgroupidactions
      parameters:
      - in: query
        name: actions
        description: When enabled, response yields additional details on users&#8217;
          access rights
        type: string
      - in: query
        name: groupId
        description: Unique numeric identifier for a group
        type: string
      responses:
        200:
          description: OK
      tags:
      - user
      - admin
      - users
      - group
      - actions
definitions: []
x-collection-name: Akamai
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