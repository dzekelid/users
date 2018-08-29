---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 0
info:
  title: Google Cloud SQL API Add Projects Project Instances Instance Users
  description: Creates a new user in a Cloud SQL instance.
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