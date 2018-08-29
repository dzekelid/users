---
swagger: "2.0"
x-collection-name: AppVeyor CI
x-complete: 1
info:
  title: App Veyor
  description: appveyor-is-a-hosted-continuous-integration-service-which-runs-on-microsoftwindows---the-appveyor-rest-api-provides-a-restful-way-to-interact-with-theappveyor-service---this-includes-managing-projects-builds-deploymentsand-the-teams-that-build-them-additional-help-and-discussion-of-the-appveyor-rest-api-is-available-athttphelp-appveyor-comdiscussionsthis-swagger-definition-is-an-unofficial-description-of-the-appveyorrest-api-maintained-at-httpsgithub-comkevinoidappveyorswaggerplease-report-any-issues-or-suggestions-for-this-swagger-definition-athttpsgithub-comkevinoidappveyorswaggerissuesnew-api-conventionsfields-which-are-missing-from-update-operations-put-requests-aretypically-reset-to-their-default-values---so-although-most-fields-are-nottechnically-required-they-should-usually-be-specified-in-practice-
  termsOfService: https://www.appveyor.com/terms-of-service/
  contact:
    name: AppVeyor Team
    url: https://www.appveyor.com/about/
    email: team@appveyor.com
  version: 0.20170106.0
host: ci.appveyor.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborators/{userId}:
    delete:
      summary: Delete Collaborators Userid
      description: Delete collaborators userid.
      operationId: deleteCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-delete
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
    get:
      summary: Get Collaborators Userid
      description: Get collaborators userid.
      operationId: getCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-get
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
    parameters:
      summary: Parameters Collaborators Userid
      description: Parameters collaborators userid.
      operationId: parametersCollaboratorsUser
      x-api-path-slug: collaboratorsuserid-parameters
      responses:
        200:
          description: OK
      tags:
      - Collaborators
      - Users
  /users:
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: Post users.
      operationId: postUsers
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
    put:
      summary: Put Users
      description: Put users.
      operationId: putUsers
      x-api-path-slug: users-put
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
  /users/{userId}:
    delete:
      summary: Delete Users Userid
      description: Delete users userid.
      operationId: deleteUsersUser
      x-api-path-slug: usersuserid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Users
    get:
      summary: Get Users Userid
      description: Get users userid.
      operationId: getUsersUser
      x-api-path-slug: usersuserid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Users
    parameters:
      summary: Parameters Users Userid
      description: Parameters users userid.
      operationId: parametersUsersUser
      x-api-path-slug: usersuserid-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Users
---