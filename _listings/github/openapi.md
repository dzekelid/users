---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers--over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories--with-the-collaborative-features-of-github-com-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code-
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
  /users/{username}/keys:
    get:
      summary: Get Users Username Keys
      description: |-
        List public keys for a user.
        Lists the verified public keys for a user. This is accessible by anyone.
      operationId: list-public-keys-for-a-userlists-the-verified-public-keys-for-a-user-this-is-accessible-by-anyone
      x-api-path-slug: usersusernamekeys-get
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
      - Keys
  /users/{username}/orgs:
    get:
      summary: Get Users Username Orgs
      description: List all public organizations for a user.
      operationId: list-all-public-organizations-for-a-user
      x-api-path-slug: usersusernameorgs-get
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
      - Orgs
  /users/{username}/received_events:
    get:
      summary: Get Users Username Received Events
      description: These are events that you'll only see public events.
      operationId: these-are-events-that-youll-only-see-public-events
      x-api-path-slug: usersusernamereceived-events-get
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
      - Received
      - Events
  /users/{username}/received_events/public:
    get:
      summary: Get Users Username Received Events Public
      description: List public events that a user has received
      operationId: list-public-events-that-a-user-has-received
      x-api-path-slug: usersusernamereceived-eventspublic-get
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
      - Received
      - Events
      - Public
  /users/{username}/repos:
    get:
      summary: Get Users Username Repos
      description: List public repositories for the specified user.
      operationId: list-public-repositories-for-the-specified-user
      x-api-path-slug: usersusernamerepos-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: type
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Repos
  /users/{username}/starred:
    get:
      summary: Get Users Username Starred
      description: List repositories being starred by a user.
      operationId: list-repositories-being-starred-by-a-user
      x-api-path-slug: usersusernamestarred-get
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
      - Starred
  /users/{username}/subscriptions:
    get:
      summary: Get Users Username Subscriptions
      description: List repositories being watched by a user.
      operationId: list-repositories-being-watched-by-a-user
      x-api-path-slug: usersusernamesubscriptions-get
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
      - Subscriptions
---