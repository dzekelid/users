---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Get Users Username Repositories
  description: |-
    All repositories owned by a user/team. This includes private
    repositories, but filtered down to the ones that the calling user has
    access to.
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{username}:
    get:
      summary: Get Users Username
      description: |-
        Gets the public information associated with a user account.

        If the user's profile is private, `location`, `website` and
        `created_on` elements are omitted.
      operationId: getUsersUsername
      x-api-path-slug: usersusername-get
      parameters:
      - in: path
        name: username
        description: The accounts username or UUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
    parameters:
      summary: Parameters Users Username
      description: Parameters users username
      operationId: parametersUsersUsername
      x-api-path-slug: usersusername-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
  /users/{username}/followers:
    get:
      summary: Get Users Username Followers
      description: Returns the list of accounts that are following this team.
      operationId: getUsersUsernameFollowers
      x-api-path-slug: usersusernamefollowers-get
      parameters:
      - in: path
        name: username
        description: The accounts username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Followers
    parameters:
      summary: Parameters Users Username Followers
      description: Parameters users username followers
      operationId: parametersUsersUsernameFollowers
      x-api-path-slug: usersusernamefollowers-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Followers
  /users/{username}/following:
    get:
      summary: Get Users Username Following
      description: Returns the list of accounts this user is following.
      operationId: getUsersUsernameFollowing
      x-api-path-slug: usersusernamefollowing-get
      parameters:
      - in: path
        name: username
        description: The users username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Following
    parameters:
      summary: Parameters Users Username Following
      description: Parameters users username following
      operationId: parametersUsersUsernameFollowing
      x-api-path-slug: usersusernamefollowing-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Following
  /users/{username}/hooks:
    get:
      summary: Get Users Username Hooks
      description: Returns a paginated list of webhooks installed on this user account.
      operationId: getUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
    parameters:
      summary: Parameters Users Username Hooks
      description: Parameters users username hooks
      operationId: parametersUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
    post:
      summary: Add Users Username Hooks
      description: |-
        Creates a new webhook on the specified user account.

        Account-level webhooks are fired for events from all repositories
        belonging to that account.

        Note that one can only register webhooks on one's own account, not that
        of others.
      operationId: postUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
  /users/{username}/hooks/{uid}:
    delete:
      summary: Delete Users Username Hooks U
      description: |-
        Deletes the specified webhook subscription from the given user
        account.
      operationId: deleteUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-delete
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    get:
      summary: Get Users Username Hooks U
      description: |-
        Returns the webhook with the specified id installed on the given
        user account.
      operationId: getUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-get
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    parameters:
      summary: Parameters Users Username Hooks U
      description: Parameters users username hooks u
      operationId: parametersUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    put:
      summary: Update Users Username Hooks U
      description: |-
        Updates the specified webhook subscription.

        The following properties can be mutated:

        * `description`
        * `url`
        * `active`
        * `events`
      operationId: putUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-put
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
  /users/{username}/pipelines_config/variables/:
    get:
      summary: Get Users Username Pipelines Config Variables
      description: Get users username pipelines config variables
      operationId: getUsersUsernamePipelinesConfigVariables
      x-api-path-slug: usersusernamepipelines-configvariables-get
      parameters:
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Pipelines
      - Config
      - Variables
    post:
      summary: Add Users Username Pipelines Config Variables
      description: Post users username pipelines config variables
      operationId: postUsersUsernamePipelinesConfigVariables
      x-api-path-slug: usersusernamepipelines-configvariables-post
      parameters:
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The variable to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Pipelines
      - Config
      - Variables
  /users/{username}/pipelines_config/variables/{variable_uuid}:
    delete:
      summary: Delete Users Username Pipelines Config Variables Variable Uu
      description: Delete users username pipelines config variables variable uu
      operationId: deleteUsersUsernamePipelinesConfigVariablesVariableUu
      x-api-path-slug: usersusernamepipelines-configvariablesvariable-uuid-delete
      parameters:
      - in: path
        name: username
        description: The account
      - in: path
        name: variable_uuid
        description: The UUID of the variable to delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Pipelines
      - Config
      - Variables
      - Variable
      - Uu
    get:
      summary: Get Users Username Pipelines Config Variables Variable Uu
      description: Get users username pipelines config variables variable uu
      operationId: getUsersUsernamePipelinesConfigVariablesVariableUu
      x-api-path-slug: usersusernamepipelines-configvariablesvariable-uuid-get
      parameters:
      - in: path
        name: username
        description: The account
      - in: path
        name: variable_uuid
        description: The UUID of the variable to retrieve
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Pipelines
      - Config
      - Variables
      - Variable
      - Uu
    put:
      summary: Update Users Username Pipelines Config Variables Variable Uu
      description: Put users username pipelines config variables variable uu
      operationId: putUsersUsernamePipelinesConfigVariablesVariableUu
      x-api-path-slug: usersusernamepipelines-configvariablesvariable-uuid-put
      parameters:
      - in: path
        name: username
        description: The account
      - in: path
        name: variable_uuid
        description: The UUID of the variable
      - in: body
        name: _body
        description: The updated variable
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Pipelines
      - Config
      - Variables
      - Variable
      - Uu
  /users/{username}/repositories:
    get:
      summary: Get Users Username Repositories
      description: |-
        All repositories owned by a user/team. This includes private
        repositories, but filtered down to the ones that the calling user has
        access to.
      operationId: getUsersUsernameRepositories
      x-api-path-slug: usersusernamerepositories-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Repositories
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