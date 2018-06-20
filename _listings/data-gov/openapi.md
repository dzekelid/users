---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/:
    get:
      summary: Get Users
      description: List all objects
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: organization
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Add Users
      description: Create a new object
      operationId: postUsers
      x-api-path-slug: users-post
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/suggest/:
    get:
      summary: Get Users Suggest
      description: Suggest users
      operationId: getUsersSuggest
      x-api-path-slug: userssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggest
  /users/{id}/followers/:
    delete:
      summary: Delete Users  Followers
      description: Unfollow an object given its ID
      operationId: deleteUsersFollowers
      x-api-path-slug: usersidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
    get:
      summary: Get Users  Followers
      description: List all followers for a given object
      operationId: getUsersFollowers
      x-api-path-slug: usersidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
    post:
      summary: Add Users  Followers
      description: Follow an user given its ID
      operationId: postUsersFollowers
      x-api-path-slug: usersidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
  /users/{user}/:
    delete:
      summary: Delete Users User
      description: Delete a given object
      operationId: deleteUsersUser
      x-api-path-slug: usersuser-delete
      parameters:
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
    get:
      summary: Get Users User
      description: Get a given object
      operationId: getUsersUser
      x-api-path-slug: usersuser-get
      parameters:
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
    put:
      summary: Put Users User
      description: Update a given object
      operationId: putUsersUser
      x-api-path-slug: usersuser-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
---