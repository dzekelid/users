---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Users Approve
  description: /users/{USER_ID}/venuehistory
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/leaderboard:
    get:
      summary: Get Users Leaderboard
      description: /users/{USER_ID}
      operationId: usersuser-id
      x-api-path-slug: usersleaderboard-get
      parameters:
      - in: query
        name: neighbors
        description: Number of friends scores to return that are adjacent to your
          score, in ranked order
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Leaderboard
  /users/requests:
    get:
      summary: Get Users Requests
      description: /users/leaderboard
      operationId: usersleaderboard
      x-api-path-slug: usersrequests-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Requests
  /users/search:
    get:
      summary: Get Users Search
      description: /users/requests
      operationId: usersrequests
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: email
        description: A comma-delimited list of email addresses to look for
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A single string to search for in users names
      - in: query
        name: phone
        description: A comma-delimited list of phone numbers to look for
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: twitterSource
        description: A single Twitter handle
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Search
    post:
      summary: Post Users Search
      description: users/search (GET)
      operationId: userssearch-get
      x-api-path-slug: userssearch-post
      parameters:
      - in: query
        name: email
        description: A comma-delimited list of email addresses to look for
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A single string to search for in users names
      - in: query
        name: phone
        description: A comma-delimited list of phone numbers to look for
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: twitterSource
        description: A single Twitter handle
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Search
  /users/self/update:
    post:
      summary: Post Users Self Update
      description: /users/{USER_ID}/unfriend
      operationId: usersuser-idunfriend
      x-api-path-slug: usersselfupdate-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: photo
        description: Photo under 100KB in multipart MIME encoding with content type
          image/jpeg, image/gif, or image/png
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
  /users/{USER_ID}:
    get:
      summary: Get Users
      description: ""
      operationId: ""
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: query
        name: USER_ID
        description: Identity of the user to get details for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{USER_ID}/approve:
    post:
      summary: Post Users Approve
      description: /users/{USER_ID}/venuehistory
      operationId: usersuser-idvenuehistory
      x-api-path-slug: usersuser-idapprove-post
      parameters:
      - in: query
        name: USER_ID
        description: The user ID of a pending friend
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Approve
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