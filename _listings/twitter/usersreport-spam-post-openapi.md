---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Report User Spam
  description: Returna users report spam
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/lookup:
    get:
      summary: User Lookup
      description: returns fully-hydrated user objects up to 100
      operationId: returns-fullyhydrated-user-objects-up-to-100
      x-api-path-slug: userslookup-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to lookup
      - in: query
        name: user_id
        description: ID of user to lookup
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/show:
    get:
      summary: Show User
      description: returns a variety of info about specified user
      operationId: returns-a-variety-of-info-about-specified-user
      x-api-path-slug: usersshow-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be shown
      - in: query
        name: user_id
        description: ID of user to be shown
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/search.json:
    get:
      summary: User Search
      description: simple relevance-based user search
      operationId: simple-relevancebased-user-search
      x-api-path-slug: userssearch-json-get
      parameters:
      - in: query
        name: count
        description: number of people to return per page
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: page
        description: specifies the page of results to receive
      - in: query
        name: q
        description: the search query to run against people search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/contributees:
    get:
      summary: User Contributees
      description: collection of users specified user can contribute to
      operationId: collection-of-users-specified-user-can-contribute-to
      x-api-path-slug: userscontributees-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user that is contributed to
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to that is contributed to
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/contributors:
    get:
      summary: User Contributors
      description: collection of users that can contribute to specified account
      operationId: collection-of-users-that-can-contribute-to-specified-account
      x-api-path-slug: userscontributors-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user contributing
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user contributing
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/report_spam:
    post:
      summary: Report User Spam
      description: Returna users report spam
      operationId: returna-users-report-spam
      x-api-path-slug: usersreport-spam-post
      parameters:
      - in: query
        name: screen_name
        description: The ID or screen_name of the user you want to report as a spammer
      - in: query
        name: user_id
        description: The ID of the user you want to report as a spammer
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
      - Spam
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