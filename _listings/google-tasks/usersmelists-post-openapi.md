---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 0
info:
  title: Google Tasks API Add Users @me Lists
  description: Creates a new task list and adds it to the authenticated user's task
    lists.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/@me/lists:
    get:
      summary: Get Users @me Lists
      description: Returns all the authenticated user's task lists.
      operationId: tasks.tasklists.list
      x-api-path-slug: usersmelists-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
    post:
      summary: Add Users @me Lists
      description: Creates a new task list and adds it to the authenticated user's
        task lists.
      operationId: tasks.tasklists.insert
      x-api-path-slug: usersmelists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
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