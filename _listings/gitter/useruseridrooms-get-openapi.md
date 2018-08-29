---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 0
info:
  title: Gitter API Get User Rooms
  version: 1.0.0
  description: List of Rooms the user is part of.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rooms/:roomId/users:
    get:
      summary: Room Users
      description: List of Users currently in the room.
      operationId: getRoomUsers
      x-api-path-slug: roomsroomidusers-get
      parameters:
      - in: query
        name: limit
        description: maximum number of users to return (default 30)
        type: string
        format: string
      - in: query
        name: q
        description: Search query
        type: string
        format: string
      - in: query
        name: skip
        description: Skip n users
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Users
  /user:
    get:
      summary: Get User
      description: Get the current user.
      operationId: getUser
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /user/:userId/rooms:
    get:
      summary: Get User Rooms
      description: List of Rooms the user is part of.
      operationId: getUserRooms
      x-api-path-slug: useruseridrooms-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Rooms
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