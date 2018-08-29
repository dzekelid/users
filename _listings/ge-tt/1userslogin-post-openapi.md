---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Users Login
  description: 'The API is based on oauth with an xauth handshake. The request body
    looks like this:'
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/users/login:
    post:
      summary: Users Login
      description: 'The API is based on oauth with an xauth handshake. The request
        body looks like this:'
      operationId: post1UsersLogin
      x-api-path-slug: 1userslogin-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Login
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