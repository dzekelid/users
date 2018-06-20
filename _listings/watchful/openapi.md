---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
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
    get:
      summary: Find SSO User By ID
      description: Returns a SSO User based on ID
      operationId: getSsoUsersById
      x-api-path-slug: ssousersid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of SSO User that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
    put:
      summary: Update A SSO User
      description: Update a SSO User
      operationId: UpdateSsoUsers
      x-api-path-slug: ssousersid-put
      parameters:
      - in: body
        name: body
        description: JSON object SsoUsers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of SSO User that needs to be updated
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
---