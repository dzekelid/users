---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Set User Profile Photo
  description: Set the user profile photo
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users.profile.set:
    post:
      summary: Set User Profile
      description: Set the profile information for a user.
      operationId: users_profile_set
      x-api-path-slug: users-profile-set-post
      parameters:
      - in: formData
        name: name
        description: Name of a single key to set
      - in: formData
        name: profile
        description: Collection of key:value pairs presented as a URL-encoded JSON
          hash
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: ID of user to change
      - in: formData
        name: value
        description: Value to set a single key to
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Users
  /users.setPresence:
    post:
      summary: Set User Presence
      description: Manually sets user presence.
      operationId: users_setPresence
      x-api-path-slug: users-setpresence-post
      parameters:
      - in: formData
        name: presence
        description: Either `auto` or `away`
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Users
  /users.info:
    get:
      summary: Get User Info
      description: Gets information about a user.
      operationId: users_info
      x-api-path-slug: users-info-get
      parameters:
      - in: query
        name: include_locale
        description: Set this to `true` to receive the locale for this user
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: user
        description: User to get info on
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Users
  /users.lookupByEmail:
    get:
      summary: Find User
      description: Find a user with an email address.
      operationId: users_lookupByEmail
      x-api-path-slug: users-lookupbyemail-get
      parameters:
      - in: query
        name: email
        description: An email address belonging to a user in the workspace
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Users
  /users.setPhoto:
    post:
      summary: Set User Profile Photo
      description: Set the user profile photo
      operationId: users_setPhoto
      x-api-path-slug: users-setphoto-post
      parameters:
      - in: formData
        name: crop_w
        description: Width/height of crop box (always square)
      - in: formData
        name: crop_x
        description: X coordinate of top-left corner of crop box
      - in: formData
        name: crop_y
        description: Y coordinate of top-left corner of crop box
      - in: formData
        name: image
        description: File contents via `multipart/form-data`
      - in: formData
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
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