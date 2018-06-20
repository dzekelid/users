---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 1
info:
  title: Ge.tt  REST API
  description: the-ge-tt-api-allows-you-to-use-ge-tt-in-your-own-applications--we-believe-that-our-users-should-be-able-to-access-their-files-and-share-their-content-in-their-platform-of-choice--by-using-the-api-developers-are-able-to-easily-put-their-own-content-or-the-content-of-their-users-online--at-the-same-time-they-are-able-to-use-ge-tts-unique-realtime-file-sharing-technology-where-files-are-available-before-they-are-even-uploaded-
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
  /1/users/me:
    get:
      summary: Users Me
      description: 'Returns your user information:'
      operationId: get1UsersMe
      x-api-path-slug: 1usersme-get
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me
---