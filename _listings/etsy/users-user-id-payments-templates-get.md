---
swagger: "2.0"
info:
  title: Etsy Get Users User Payments Templates
  description: Retrieves a set of PaymentTemplate objects associated to a User.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/payments/templates:
    get:
      summary: Get Users User Payments Templates
      description: Retrieves a set of PaymentTemplate objects associated to a User
      operationId: getUsersUserPaymentsTemplates
      responses:
        200:
          description: OK
      tags:
      - users
      - payments
      - templates
definitions: []
x-collection-name: Etsy
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