---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Delete A Specific SSO User
  description: Delete a specific SSO User
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ssousers:
    get:
      summary: Get A List Of SSO Users
      description: Returns a list of SSO Users
      operationId: getSsoUsers
      x-api-path-slug: ssousers-get
      responses:
        200:
          description: OK
      tags:
      - Ssousers
    post:
      summary: Create A SSO User
      description: Create a SSO User
      operationId: CreateSsoUsers
      x-api-path-slug: ssousers-post
      parameters:
      - in: body
        name: body
        description: JSON object SsoUsers
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ssousers
  /ssousers/{id}:
    delete:
      summary: Delete A Specific SSO User
      description: Delete a specific SSO User
      operationId: deleteSsoUserById
      x-api-path-slug: ssousersid-delete
      parameters:
      - in: path
        name: id
        description: ID of SSO User that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
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