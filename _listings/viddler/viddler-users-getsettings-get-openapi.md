---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 0
info:
  title: Viddler  API Users GetSettings
  description: Return account settings.
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.users.getPlayerBranding:
    get:
      summary: Users GetPlayerBranding
      description: Returns your player branding configuration.
      operationId: users-getplayerbranding
      x-api-path-slug: viddler-users-getplayerbranding-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetPlayerBranding
  viddler.users.getProfile:
    get:
      summary: Users GetProfile
      description: Get the public information for a profile. Can only get profile
        information for public profiles.
      operationId: users-getprofile
      x-api-path-slug: viddler-users-getprofile-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: user
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetProfile
  viddler.users.getSettings:
    get:
      summary: Users GetSettings
      description: Return account settings.
      operationId: users-getsettings
      x-api-path-slug: viddler-users-getsettings-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetSettings
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