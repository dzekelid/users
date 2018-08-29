---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Get Getuser
  description: The method getuser returns information about a user such as prefered
    language, prefered units, and list of devices.
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getuser:
    get:
      summary: Get Getuser
      description: The method getuser returns information about a user such as prefered
        language, prefered units, and list of devices.
      operationId: getuser
      x-api-path-slug: getuser-get
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