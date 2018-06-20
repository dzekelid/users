---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Move User's Folder
  description: "Moves all of the owned content from within one user\u2019s folder
    into a new folder in another user\u2019s account. You can move folders across
    users as long as the you have administrative permissions and the \u2018source\u2019
    user owns the folders. To move everything from the root folder, use \u201C0\u201D
    which always represents the root folder of a Box account."
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
    put:
      summary: Update User, Change User's Login
      description: "Used to edit the settings and information about a user. This method
        only works for enterprise admins. To roll a user out of the enterprise (and
        convert them to a standalone free user), update the special enterprise attribute
        to be null.\n\nUsed to convert one of the user\u2019s confirmed email aliases
        into the user\u2019s primary login."
      operationId: updateUser
      x-api-path-slug: usersuser-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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
    delete:
      summary: Delete User
      description: Deletes a user in an enterprise account.
      operationId: deleteUser
      x-api-path-slug: usersuser-id-delete
      parameters:
      - in: query
        name: force
      - in: query
        name: notify
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
  /users/{USER_ID}/folders/{FOLDER_ID}:
    put:
      summary: Move User's Folder
      description: "Moves all of the owned content from within one user\u2019s folder
        into a new folder in another user\u2019s account. You can move folders across
        users as long as the you have administrative permissions and the \u2018source\u2019
        user owns the folders. To move everything from the root folder, use \u201C0\u201D
        which always represents the root folder of a Box account."
      operationId: updateUserFolder
      x-api-path-slug: usersuser-idfoldersfolder-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FOLDER_ID
      - in: query
        name: notify
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Folders
      - Folder
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