---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API List users in group category
  description: List users in group category.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/users:
    get:
      summary: List groups users
      description: List groups users.
      operationId: list-groups-users
      x-api-path-slug: groupsgroup-idusers-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cavatar_urlu201d: Include users&#39; avatar_urls'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
  /groups/{group_id}/users/user_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idusersuser-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idusersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idusersuser-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
  /group_categories/{group_category_id}/users:
    get:
      summary: List users in group category
      description: List users in group category.
      operationId: list-users-in-group-category
      x-api-path-slug: group-categoriesgroup-category-idusers-get
      parameters:
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: unassigned
        description: Set this value to true if you wish only to search unassigned
          users in thengroup category
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
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