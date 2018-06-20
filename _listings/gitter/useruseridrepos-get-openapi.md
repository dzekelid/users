---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 0
info:
  title: Gitter API User Repos
  version: 1.0.0
  description: List of the user's GitHub Repositories and their respective Room if
    available.
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
  /user/:userId/rooms/:roomId/unreadItems:
    get:
      summary: Get User Unread Items
      description: You can retrieve unread items and mentions using the following
        endpoint.
      operationId: getUserUnreadItems
      x-api-path-slug: useruseridroomsroomidunreaditems-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Messages
      - Unread
  /user/:userId/orgs:
    get:
      summary: User Orgs
      description: List of the user's GitHub Organisations and their respective Room
        if available.
      operationId: getUserOrgs
      x-api-path-slug: useruseridorgs-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Organizations
  /user/:userId/repos:
    get:
      summary: User Repos
      description: List of the user's GitHub Repositories and their respective Room
        if available.
      operationId: getUserRepos
      x-api-path-slug: useruseridrepos-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Repositories
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