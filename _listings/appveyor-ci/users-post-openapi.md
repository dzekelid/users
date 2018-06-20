---
swagger: "2.0"
x-collection-name: AppVeyor CI
x-complete: 0
info:
  title: App Veyor Post Users
  description: Post users.
  termsOfService: https://www.appveyor.com/terms-of-service/
  contact:
    name: AppVeyor Team
    url: https://www.appveyor.com/about/
    email: team@appveyor.com
  version: 0.20170106.0
host: ci.appveyor.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborators/{userId}:
    delete:
      summary: Delete Collaborators Userid
      description: Delete collaborators userid.
      operationId: deleteCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-delete
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
    get:
      summary: Get Collaborators Userid
      description: Get collaborators userid.
      operationId: getCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-get
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
    parameters:
      summary: Parameters Collaborators Userid
      description: Parameters collaborators userid.
      operationId: parametersCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-parameters
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
  /users:
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: Post users.
      operationId: postUsers
      x-api-path-slug: users-post
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