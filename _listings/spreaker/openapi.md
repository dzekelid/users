---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/{query}:
    get:
      summary: Search users, shows and episodes
      description: Search users, shows and episodes
      operationId: getSearchQuery
      x-api-path-slug: searchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users
      - ""
      - Shows
      - Episodes
  /users/search/{query}:
    get:
      summary: Search Users
      description: This API allows to find users.
      operationId: getUsersSearchQuery
      x-api-path-slug: userssearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users
---