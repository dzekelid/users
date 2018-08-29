---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Users Request
  description: /users/{USER_ID}/deny
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
  /users/{USER_ID}/badges:
    get:
      summary: Get Users Badges
      description: users/search (POST)
      operationId: userssearch-post
      x-api-path-slug: usersuser-idbadges-get
      parameters:
      - in: query
        name: USER_ID
        description: ID for user to view badges for
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
      - Badges
  /users/{USER_ID}/checkins:
    get:
      summary: Get Users Checkins
      description: /users/{USER_ID}/badges
      operationId: usersuser-idbadges
      x-api-path-slug: usersuser-idcheckins-get
      parameters:
      - in: query
        name: afterTimestamp
        description: Retrieve the first results to follow these seconds since epoch
      - in: query
        name: beforeTimestamp
        description: Retrieve the first results prior to these seconds since epoch
      - in: query
        name: limit
        description: Number of results to return, up to 250
      - in: query
        name: offset
        description: The number of results to skip
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
      - Checkins
  /users/{USER_ID}/deny:
    post:
      summary: Post Users Deny
      description: /users/{USER_ID}/approve
      operationId: usersuser-idapprove
      x-api-path-slug: usersuser-iddeny-post
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
      - Deny
  /users/{USER_ID}/friends:
    get:
      summary: Get Users Friends
      description: /users/{USER_ID}/checkins
      operationId: usersuser-idcheckins
      x-api-path-slug: usersuser-idfriends-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: USER_ID
        description: Identity of the user to get friends of
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
      - Friends
  /users/{USER_ID}/lists:
    get:
      summary: Get Users Lists
      description: /users/{USER_ID}/friends
      operationId: usersuser-idfriends
      x-api-path-slug: usersuser-idlists-get
      parameters:
      - in: query
        name: group
        description: Can be created (lists created by this user), edited (other peoples
          lists this user has edited), followed (lists this user follows), friends
          (lists from this users friends), and suggested (lists relevant to the users
          current location)
      - in: query
        name: ll
        description: Location of the user, required in order to receive the suggested
          group
      - in: query
        name: USER_ID
        description: Identity of the user to get lists for
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
      - Lists
  /users/{USER_ID}/mayorships:
    get:
      summary: Get Users Mayorships
      description: /users/{USER_ID}/lists
      operationId: usersuser-idlists
      x-api-path-slug: usersuser-idmayorships-get
      parameters:
      - in: query
        name: USER_ID
        description: Identity of the user to get mayorships for
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
      - Mayorships
  /users/{USER_ID}/photos:
    get:
      summary: Get Users Photos
      description: /users/{USER_ID}/mayorships
      operationId: usersuser-idmayorships
      x-api-path-slug: usersuser-idphotos-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
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
      - Photos
  /users/{USER_ID}/request:
    post:
      summary: Post Users Request
      description: /users/{USER_ID}/deny
      operationId: usersuser-iddeny
      x-api-path-slug: usersuser-idrequest-post
      parameters:
      - in: query
        name: USER_ID
        description: The user ID to which a request will be sent
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
      - Request
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