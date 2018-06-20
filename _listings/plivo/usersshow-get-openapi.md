---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Get Users Show
  description: Returns the profile information for a specified user.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get Users
      description: Returns the profile information for the current user.
      operationId: returns-the-profile-information-for-the-current-user
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/:id/followers:
    get:
      summary: Get Users Followers
      description: Returns a list of users who follow the specified user.
      operationId: returns-a-list-of-users-who-follow-the-specified-user
      x-api-path-slug: usersidfollowers-get
      parameters:
      - in: query
        name: id (required)
        description: ID of the user
      - in: query
        name: page
        description: Return the specified page of the resource
      - in: query
        name: rpp
        description: Results Per Page, default 20, max 100
      responses:
        200:
          description: OK
      tags:
      - Users
      - :id
      - Followers
  /users/:id/friends:
    post:
      summary: Post Users Friends
      description: Add the user to the list of followers.
      operationId: add-the-user-to-the-list-of-followers
      x-api-path-slug: usersidfriends-post
      parameters:
      - in: query
        name: id (required)
        description: ID of the User to add to the followers list
      responses:
        200:
          description: OK
      tags:
      - Users
      - :id
      - Friends
  /users/search:
    get:
      summary: Get Users Search
      description: Return listing of ten (up to one hundred) users from search results
        for a specified search term.
      operationId: return-listing-of-ten-up-to-one-hundred-users-from-search-results-for-a-specified-search-term
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: term (required)
        description: A keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Users
      - Search
  /users/show:
    get:
      summary: Get Users Show
      description: Returns the profile information for a specified user.
      operationId: returns-the-profile-information-for-a-specified-user
      x-api-path-slug: usersshow-get
      parameters:
      - in: query
        name: email
        description: Return information for the user with the specified email address
      - in: query
        name: id
        description: Return information for the specified user ID
      - in: query
        name: username
        description: Return information for the user with the specified username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Show
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