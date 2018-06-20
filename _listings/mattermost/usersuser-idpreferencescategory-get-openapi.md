---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API List a user's preferences by category
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get users
      description: |-
        Get a page of a list of users. Based on query string parameters, select users from a team, channel, or select users not in a specific channel.

        Since server version 4.0, some basic sorting is available using the `sort` query parameter. Sorting is currently only supported when selecting users on a team.
        ##### Permissions
        Requires an active session and (if specified) membership to the channel or team being selected from.
      operationId: get-a-page-of-a-list-of-users-based-on-query-string-parameters-select-users-from-a-team-channel-or-s
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: in_channel
        description: The ID of the channel to get users for
      - in: query
        name: in_team
        description: The ID of the team to get users for
      - in: query
        name: not_in_channel
        description: The ID of the channel to exclude users for
      - in: query
        name: not_in_team
        description: The ID of the team to exclude users for
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of users per page
      - in: query
        name: sort
        description: Sort is only available in conjunction with certain options below
      - in: query
        name: without_team
        description: Whether or not to list users that are not on any team
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/ids:
    post:
      summary: Get users by ids
      description: |-
        Get a list of users based on a provided list of user ids.
        ##### Permissions
        Requires an active session but no other permissions.
      operationId: get-a-list-of-users-based-on-a-provided-list-of-user-ids-permissionsrequires-an-active-session-but-n
      x-api-path-slug: usersids-post
      parameters:
      - in: body
        name: body
        description: List of user ids
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - By
      - Ids
  /users/usernames:
    post:
      summary: Get users by usernames
      description: |-
        Get a list of users based on a provided list of usernames.
        ##### Permissions
        Requires an active session but no other permissions.
      operationId: get-a-list-of-users-based-on-a-provided-list-of-usernames-permissionsrequires-an-active-session-but-
      x-api-path-slug: usersusernames-post
      parameters:
      - in: body
        name: body
        description: List of usernames
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - By
      - Usernames
  /users/search:
    post:
      summary: Search users
      description: |-
        Get a list of users based on search criteria provided in the request body. Searches are typically done against username, full name, nickname and email unless otherwise configured by the server.
        ##### Permissions
        Requires an active session and `read_channel` and/or `view_team` permissions for any channels or teams specified in the request body.
      operationId: get-a-list-of-users-based-on-search-criteria-provided-in-the-request-body-searches-are-typically-don
      x-api-path-slug: userssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users
  /users/autocomplete:
    get:
      summary: Autocomplete users
      description: |-
        Get a list of users for the purpose of autocompleting based on the provided search term. Specify a combination of `team_id` and `channel_id` to filter results further.
        ##### Permissions
        Requires an active session and `view_team` and `read_channel` on any teams or channels used to filter the results further.
      operationId: get-a-list-of-users-for-the-purpose-of-autocompleting-based-on-the-provided-search-term-specify-a-co
      x-api-path-slug: usersautocomplete-get
      parameters:
      - in: query
        name: channel_id
        description: Channel ID
      - in: query
        name: name
        description: Username, nickname first name or last name
      - in: query
        name: team_id
        description: Team ID
      responses:
        200:
          description: OK
      tags:
      - Autocomplete
      - Users
  /users/{user_id}/roles:
    put:
      summary: Update a user's roles
      description: |-
        Update a user's system-level roles. Valid user roles are "system_user", "system_admin" or both of them. Overwrites any previously assigned system-level roles.
        ##### Permissions
        Must have the `manage_roles` permission.
      operationId: update-a-users-systemlevel-roles-valid-user-roles-are-system-user-system-admin-or-both-of-them-overw
      x-api-path-slug: usersuser-idroles-put
      parameters:
      - in: body
        name: roles
        description: Space-delimited system roles to assign to the user
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Roles
  /users/{user_id}/image:
    get:
      summary: Get user's profile image
      description: |-
        Get a user's profile image based on user_id string parameter.
        ##### Permissions
        Must be logged in.
      operationId: get-a-users-profile-image-based-on-user-id-string-parameter-permissionsmust-be-logged-in
      x-api-path-slug: usersuser-idimage-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Profile
      - Image
    post:
      summary: Set user's profile image
      description: |-
        Set a user's profile image based on user_id string parameter.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: set-a-users-profile-image-based-on-user-id-string-parameter-permissionsmust-be-logged-in-as-the-user
      x-api-path-slug: usersuser-idimage-post
      parameters:
      - in: formData
        name: image
        description: The image to be uploaded
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Set
      - Users
      - Profile
      - Image
  /users/{user_id}/mfa:
    put:
      summary: Update a user's MFA
      description: |-
        Activates multi-factor authentication for the user if `activate` is true and a valid `code` is provided. If activate is false, then `code` is not required and multi-factor authentication is disabled for the user.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: activates-multifactor-authentication-for-the-user-if-activate-is-true-and-a-valid-code-is-provided-i
      x-api-path-slug: usersuser-idmfa-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - MFA
  /users/{user_id}/password:
    put:
      summary: Update a user's password
      description: |-
        Update a user's password. New password must meet password policy set by server configuration. Current password is required if you're updating your own password.
        ##### Permissions
        Must be logged in as the user the password is being changed for or have `manage_system` permission.
      operationId: update-a-users-password-new-password-must-meet-password-policy-set-by-server-configuration-current-p
      x-api-path-slug: usersuser-idpassword-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Password
  /users/{user_id}/sessions:
    get:
      summary: Get user's sessions
      description: |-
        Get a list of sessions by providing the user GUID. Sensitive information will be sanitized out.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: get-a-list-of-sessions-by-providing-the-user-guid-sensitive-information-will-be-sanitized-out-permis
      x-api-path-slug: usersuser-idsessions-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Sessions
  /users/{user_id}/audits:
    get:
      summary: Get users audits
      description: |-
        Get a list of audit by providing the user GUID.
        ##### Permissions
        Must be logged in as the user or have the `edit_other_users` permission.
      operationId: get-a-list-of-audit-by-providing-the-user-guid-permissionsmust-be-logged-in-as-the-user-or-have-the-
      x-api-path-slug: usersuser-idaudits-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Audits
  /users/{user_id}/auth:
    put:
      summary: Update a users authentication method
      description: |-
        Updates a user's authentication method. This can be used to change them to/from LDAP authentication for example.

        __Minimum server version__: 4.6
        ##### Permissions
        Must have the `edit_other_users` permission.
      operationId: updates-a-users-authentication-method-this-can-be-used-to-change-them-tofrom-ldap-authentication-for
      x-api-path-slug: usersuser-idauth-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Authentication
      - Method
  /users/{user_id}/teams:
    get:
      summary: Get a user's teams
      description: |-
        Get a list of teams that a user is on.
        ##### Permissions
        Must be authenticated as the user or have the `manage_system` permission.
      operationId: get-a-list-of-teams-that-a-user-is-on-permissionsmust-be-authenticated-as-the-user-or-have-the-manag
      x-api-path-slug: usersuser-idteams-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Teams
  /teams/{team_id}/members/batch:
    post:
      summary: Add multiple users to team
      description: |-
        Add a number of users to the team by user_id.
        ##### Permissions
        Must be authenticated. Authenticated user must have the `add_user_to_team` permission.
      operationId: add-a-number-of-users-to-the-team-by-user-id-permissionsmust-be-authenticated-authenticated-user-mus
      x-api-path-slug: teamsteam-idmembersbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Users
      - To
      - Team
  /teams/{team_id}/invite/email:
    post:
      summary: Invite users to the team by email
      description: |-
        Invite users to the existing team usign the user's email.
        ##### Permissions
        Must have `invite_to_team` permission for the team.
      operationId: invite-users-to-the-existing-team-usign-the-users-email-permissionsmust-have-invite-to-team-permissi
      x-api-path-slug: teamsteam-idinviteemail-post
      parameters:
      - in: body
        name: body
        description: List of users email
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Users
      - To
      - Team
      - By
      - Email
  /users/{user_id}/preferences:
    get:
      summary: Get the user's preferences
      description: |-
        Get a list of the user's preferences.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: get-a-list-of-the-users-preferences-permissionsmust-be-logged-in-as-the-user-being-updated-or-have-t
      x-api-path-slug: usersuser-idpreferences-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Preferences
    put:
      summary: Save the user's preferences
      description: |-
        Save a list of the user's preferences.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: save-a-list-of-the-users-preferences-permissionsmust-be-logged-in-as-the-user-being-updated-or-have-
      x-api-path-slug: usersuser-idpreferences-put
      parameters:
      - in: body
        name: body
        description: List of preference object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Save
      - Users
      - Preferences
  /users/{user_id}/preferences/delete:
    post:
      summary: Delete user's preferences
      description: |-
        Delete a list of the user's preferences.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: delete-a-list-of-the-users-preferences-permissionsmust-be-logged-in-as-the-user-being-updated-or-hav
      x-api-path-slug: usersuser-idpreferencesdelete-post
      parameters:
      - in: body
        name: body
        description: List of preference object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Preferences
  /users/{user_id}/preferences/{category}:
    get:
      summary: List a user's preferences by category
      description: |-
        Lists the current user's stored preferences in the given category.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: lists-the-current-users-stored-preferences-in-the-given-category-permissionsmust-be-logged-in-as-the
      x-api-path-slug: usersuser-idpreferencescategory-get
      parameters:
      - in: path
        name: category
        description: The category of a group of preferences
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Users
      - Preferences
      - By
      - Category
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