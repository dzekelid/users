---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Users:
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
    x-related-model:
      summary: X-related-model Users
      description: X-related-model users.
      operationId: x-related-modelUsers
      x-api-path-slug: users-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Users
  /Users/{UserID}:
    get:
      summary: Get Users User
      description: Get users user.
      operationId: getUsersUser
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: UserID
      responses:
        200:
          description: OK
      tags:
      - Users
      - UserID
    x-related-model:
      summary: X-related-model Users User
      description: X-related-model users user.
      operationId: x-related-modelUsersUser
      x-api-path-slug: usersuserid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Users
      - UserID
---