---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 1
info:
  title: Cloud SQL Administration
  description: creates-and-configures-cloud-sql-instances-which-provide-fullymanaged-mysql-databases-
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances/{instance}/users:
    delete:
      summary: Delete Projects Project Instances Instance Users
      description: Deletes a user from a Cloud SQL instance.
      operationId: sql.users.delete
      x-api-path-slug: projectsprojectinstancesinstanceusers-delete
      parameters:
      - in: query
        name: host
        description: Host of the user in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: query
        name: name
        description: Name of the user in the instance
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    get:
      summary: Get Projects Project Instances Instance Users
      description: Lists users in the specified Cloud SQL instance.
      operationId: sql.users.list
      x-api-path-slug: projectsprojectinstancesinstanceusers-get
      parameters:
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    post:
      summary: Add Projects Project Instances Instance Users
      description: Creates a new user in a Cloud SQL instance.
      operationId: sql.users.insert
      x-api-path-slug: projectsprojectinstancesinstanceusers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    put:
      summary: Put Projects Project Instances Instance Users
      description: Updates an existing user in a Cloud SQL instance.
      operationId: sql.users.update
      x-api-path-slug: projectsprojectinstancesinstanceusers-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: host
        description: Host of the user in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: query
        name: name
        description: Name of the user in the instance
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
      - Users
---