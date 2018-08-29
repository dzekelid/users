---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Get Users Username Gists
  description: List a users gists.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/users:
    get:
      summary: Get Search Users
      description: Search users.
      operationId: search-users
      x-api-path-slug: searchusers-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: The search terms
      - in: query
        name: sort
        description: If not provided, results are sorted by best match
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users
  /users:
    get:
      summary: Get Users
      description: |-
        Get all users.
        This provides a dump of every user, in the order that they signed up for GitHub.
        Note: Pagination is powered exclusively by the since parameter. Use the Link
        header to get the URL for the next page of users.
      operationId: get-all-usersthis-provides-a-dump-of-every-user-in-the-order-that-they-signed-up-for-githubnote-pagi
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: since
        description: The integer ID of the last User that youve seen
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{username}:
    get:
      summary: Get Users Username
      description: Get a single user.
      operationId: get-a-single-user
      x-api-path-slug: usersusername-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
  /users/{username}/events:
    get:
      summary: Get Users Username Events
      description: If you are authenticated as the given user, you will see your private
        events. Otherwise, you'll only see public events.
      operationId: if-you-are-authenticated-as-the-given-user-you-will-see-your-private-events-otherwise-youll-only-see
      x-api-path-slug: usersusernameevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Events
  /users/{username}/events/orgs/{org}:
    get:
      summary: Get Users Username Events Orgs Org
      description: This is the user's organization dashboard. You must be authenticated
        as the user to view this.
      operationId: this-is-the-users-organization-dashboard-you-must-be-authenticated-as-the-user-to-view-this
      x-api-path-slug: usersusernameeventsorgsorg-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Events
      - Orgs
      - Org
  /users/{username}/followers:
    get:
      summary: Get Users Username Followers
      description: List a user's followers
      operationId: list-a-users-followers
      x-api-path-slug: usersusernamefollowers-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Followers
  /users/{username}/following/{targetUser}:
    get:
      summary: Get Users Username Following Targetuser
      description: Check if one user follows another.
      operationId: check-if-one-user-follows-another
      x-api-path-slug: usersusernamefollowingtargetuser-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: targetUser
        description: Name of user
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Following
      - Targetuser
  /users/{username}/gists:
    get:
      summary: Get Users Username Gists
      description: List a users gists.
      operationId: list-a-users-gists
      x-api-path-slug: usersusernamegists-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: since
        description: 'The time should be passed in as UTC in the ISO 8601 format:
          YYYY-MM-DDTHH:MM:SSZ'
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Gists
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