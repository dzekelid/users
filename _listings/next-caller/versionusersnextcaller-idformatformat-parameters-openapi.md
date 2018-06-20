---
swagger: "2.0"
x-collection-name: Next Caller
x-complete: 0
info:
  title: Next Caller Parameters Version Users Nextcaller Format Format
  description: Parameters version users nextcaller format format.
  version: 1.0.0
host: api.sandbox.nextcaller.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/users/{nextcaller_id}/?format={format}:
    parameters:
      summary: Parameters Version Users Nextcaller Format Format
      description: Parameters version users nextcaller format format.
      operationId: parametersVersionUsersNextcallerFormatFormat
      x-api-path-slug: versionusersnextcaller-idformatformat-parameters
      responses:
        200:
          description: OK
      tags:
      - Version
      - Users
      - Nextcaller
      - Id
      - ?format=format
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