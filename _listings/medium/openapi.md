---
swagger: "2.0"
x-collection-name: Medium
x-complete: 1
info:
  title: Medium.com
  description: mediums-unofficial-api-documentation-using-openapi-specification--official-apiofficial-api-document-can-also-be-viewed-for-most-up-to-date-api-spec-at-httpsgithub-commediummediumapidocshttpsgithub-commediummediumapidocs-developer-blog--welcome-to-the-medium-apihttpsmedium-comblogwelcometothemediumapi3418f956552
  termsOfService: https://medium.com/@feerst/2b405a832a2f
  contact:
    name: Hossain Khan
    url: https://github.com/amardeshbd/medium-api-specification
  version: 1.0.0
host: api.medium.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{authorId}/posts:
    post:
      summary: Create User Post
      description: "Creates a post on the authenticated user\u2019s profile."
      operationId: users.authorId.posts.post
      x-api-path-slug: usersauthoridposts-post
      parameters:
      - in: path
        name: authorId
        description: authorId is the user id of the authenticated user
      - in: body
        name: body
        description: Creates a post for user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Author
      - Posts
  /users/{userId}/publications:
    get:
      summary: User's publications
      description: Returns a full list of publications that the user is related to
        in some way. This includes all publications the user is subscribed to, writes
        to, or edits.
      operationId: users.userId.publications.get
      x-api-path-slug: usersuseridpublications-get
      parameters:
      - in: path
        name: userId
        description: A unique identifier for the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Publications
---