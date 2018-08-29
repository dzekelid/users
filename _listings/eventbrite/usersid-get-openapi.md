---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Users
  description: Returns a user for the specified user as user. If you want to get details
    about the currently authenticated user, use /users/me/.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/me/notifications/:
    get:
      summary: Get Users Me Notifications
      description: Gets a paginated response of notification objects for a determined
        user.
      operationId: getUsersMeNotifications
      x-api-path-slug: usersmenotifications-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me
      - Notifications
  /users/:user_id/organizations/:
    get:
      summary: Get Users User Organizations
      description: |-
        Returns a continuated list of organizations
        accessible to the current user.
      operationId: getUsersUserOrganizations
      x-api-path-slug: usersuser-idorganizations-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Organizations
  /users/:user_id/tracking_beacons/:
    get:
      summary: Get Users User Tracking Beacons
      description: Returns the list of tracking_beacon for the user :user_id
      operationId: getUsersUserTrackingBeacons
      x-api-path-slug: usersuser-idtracking-beacons-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Tracking
      - Beacons
  /users/{id}/:
    get:
      summary: Get Users
      description: Returns a user for the specified user as user. If you want to get
        details about the currently authenticated user, use /users/me/.
      operationId: getUsers
      x-api-path-slug: usersid-get
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