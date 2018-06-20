---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 1
info:
  title: Launch Darkly
  description: build-custom-integrations-with-the-launchdarkly-rest-api
  termsOfService: https://launchdarkly.com/terms
  contact:
    name: LaunchDarkly Support
    url: https://support.launchdarkly.com
    email: support@launchdarkly.com
  version: 2.0.0
host: app.launchdarkly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{projectKey}/{environmentKey}:
    get:
      summary: List all users in the environment.
      description: List all users in the environment..
      operationId: getUsers
      x-api-path-slug: usersprojectkeyenvironmentkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
  /users/{projectKey}/{environmentKey}/{userKey}:
    delete:
      summary: Delete a user by ID
      description: Delete a user by id.
      operationId: deleteUser
      x-api-path-slug: usersprojectkeyenvironmentkeyuserkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
      - UserKey
    get:
      summary: Get a user by key.
      description: Get a user by key..
      operationId: getUser
      x-api-path-slug: usersprojectkeyenvironmentkeyuserkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
      - UserKey
  /users/{projectKey}/{environmentKey}/{userKey}/flags:
    get:
      summary: Lists the current flag settings for a given user.
      description: Lists the current flag settings for a given user..
      operationId: getUserFlagSettings
      x-api-path-slug: usersprojectkeyenvironmentkeyuserkeyflags-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
      - UserKey
      - Flags
  /users/{projectKey}/{environmentKey}/{userKey}/flags/{featureFlagKey}:
    get:
      summary: Get a user by key.
      description: Get a user by key..
      operationId: getUserFlagSetting
      x-api-path-slug: usersprojectkeyenvironmentkeyuserkeyflagsfeatureflagkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
      - UserKey
      - Flags
      - FeatureFlagKey
    put:
      summary: Specifically enable or disable a feature flag for a user based on their
        key.
      description: Specifically enable or disable a feature flag for a user based
        on their key..
      operationId: putFlagSetting
      x-api-path-slug: usersprojectkeyenvironmentkeyuserkeyflagsfeatureflagkey-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
      - UserKey
      - Flags
      - FeatureFlagKey
---