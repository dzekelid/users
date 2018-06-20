---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Users
  description: List users Retrieve a list of user objects.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/{id}/registeredUsers:
    get:
      summary: List Registered Users
      description: List registeredUsers Retrieve a list of users that are registered
        users of the device.
      operationId: ListRegisteredUsers
      x-api-path-slug: devicesidregisteredusers-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Users
  /users:
    get:
      summary: List Users
      description: List users Retrieve a list of user objects.
      operationId: ListUsers
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - List
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