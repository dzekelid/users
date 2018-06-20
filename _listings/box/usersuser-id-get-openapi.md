---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get User's Info
  description: Retrieves information about a user in the enterprise. Requires enterprise
    administration authorization.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    post:
      summary: Create User
      description: Used to provision a new user in an enterprise. This method only
        works for enterprise admins.
      operationId: createUser
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
    get:
      summary: Get Enterprise Users
      description: Returns a list of all users for the Enterprise along with their
        user_id, public_name, and login.
      operationId: getEnterpriseUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: filter_term
        description: A string used to filter the results to only users starting with
          the filter_term in either the name or the login
      - in: query
        name: limit
        description: The number of records to return
      - in: query
        name: offset
        description: The record at which to start
      - in: query
        name: user_type
        description: The type of user to search for
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
  /users/me:
    get:
      summary: Get Current User
      description: Retrieves information about the user who is currently logged in
        i.e. the user for whom this auth token was generated.
      operationId: getCurrentUser
      x-api-path-slug: usersme-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - Me
  /users/{USER_ID}:
    get:
      summary: Get User's Info
      description: Retrieves information about a user in the enterprise. Requires
        enterprise administration authorization.
      operationId: getUser
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
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