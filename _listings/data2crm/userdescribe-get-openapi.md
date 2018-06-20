---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM DESCRIBE for User
  description: Returns describe for users
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user:
    get:
      summary: GET for User
      description: Returns all users from the system
      operationId: getUserCollection
      x-api-path-slug: user-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: POST for User
      description: Add user into the system
      operationId: createUserEntity
      x-api-path-slug: user-post
      parameters:
      - in: body
        name: body
        description: Add user into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
  /user/count:
    get:
      summary: COUNT for User
      description: Count all users from the system
      operationId: getUserCountCollection
      x-api-path-slug: usercount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Count
  /user/describe:
    get:
      summary: DESCRIBE for User
      description: Returns describe for users
      operationId: getUserDescribe
      x-api-path-slug: userdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Describe
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