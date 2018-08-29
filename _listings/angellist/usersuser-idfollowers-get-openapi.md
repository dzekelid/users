---
swagger: "2.0"
x-collection-name: AngelList
x-complete: 0
info:
  title: AngelList Get User Followers
  description: Get User Followers
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/{tag_id}/users:
    get:
      summary: Get Users by Tag
      description: Get Users by Tag
      operationId: tagUsers
      x-api-path-slug: tagstag-idusers-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
      - Users
  /users/search:
    get:
      summary: User Search
      description: User Search
      operationId: users
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
  /users/{user_id}:
    get:
      summary: Get User
      description: Get User
      operationId: user
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
  /users/{user_id}/followers:
    get:
      summary: Get User Followers
      description: Get User Followers
      operationId: userFollowers
      x-api-path-slug: usersuser-idfollowers-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
      - Followers
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