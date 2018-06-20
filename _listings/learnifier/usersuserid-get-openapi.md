---
swagger: "2.0"
x-collection-name: Learnifier
x-complete: 0
info:
  title: Learnifier User information
  version: 1.1.0
  description: Returns information about a user
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extuser:
    get:
      summary: Gets a user by external id
      description: Gets a user by external id.
      operationId: extuser.get
      x-api-path-slug: extuser-get
      parameters:
      - in: query
        name: extid
        description: The external id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
  /globalusergroups:
    get:
      summary: List Global User Groups.
      description: Returns a list of Global User Groups. Global User Groups are set
        up for the realm, and will generate groups that can be used on the client
        level.
      operationId: globalusergroups.get
      x-api-path-slug: globalusergroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /globalusergroups/{groupid}/members:
    get:
      summary: List of all users in group.
      description: Returns a list of all members in User Groups that are based on
        the Global Group with this groupid.
      operationId: globalusergroups.groupid.members.get
      x-api-path-slug: globalusergroupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /orgunits/{orgid}/usergroups:
    get:
      summary: List User Groups.
      description: Returns a list of User Groups for the org unit.
      operationId: orgunits.orgid.usergroups.get
      x-api-path-slug: orgunitsorgidusergroups-get
      parameters:
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
    post:
      summary: Create a User Group.
      description: Create a User Group.
      operationId: orgunits.orgid.usergroups.post
      x-api-path-slug: orgunitsorgidusergroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
  /orgunits/{orgid}/usergroups/{groupid}:
    get:
      summary: Get user group
      description: Returns single User Group.
      operationId: orgunits.orgid.usergroups.groupid.get
      x-api-path-slug: orgunitsorgidusergroupsgroupid-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
      - Groupid
  /users:
    get:
      summary: Lists all users
      description: Lists all users. Only api callers that have full access can call
        this method.
      operationId: users.get
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of users to return
      - in: query
        name: offset
        description: The offset to start listing users from
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Adds a user
      description: Adds a user. No two users can have the same email address. Email
        is saved WITH case but compared regardless of case. Email can be changed for
        a user assuming it doesn't cause a conflict.
      operationId: users.post
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}:
    get:
      summary: User information
      description: Returns information about a user
      operationId: users.userid.get
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: userid
        description: A user id
      responses:
        200:
          description: OK
      tags:
      - Users
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