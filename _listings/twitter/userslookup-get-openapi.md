---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter User Lookup
  description: returns fully-hydrated user objects up to 100
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/lookup:
    get:
      summary: User Lookup
      description: returns fully-hydrated user objects up to 100
      operationId: returns-fullyhydrated-user-objects-up-to-100
      x-api-path-slug: userslookup-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to lookup
      - in: query
        name: user_id
        description: ID of user to lookup
      responses:
        200:
          description: OK
      tags:
      - Social
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