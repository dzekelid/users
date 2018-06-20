---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Update User
  version: 1.0.0
  description: Updates the name and/or the path of the specified IAM user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateUser:
    get:
      summary: Create User
      description: Creates a new IAM user for your AWS account.
      operationId: createUser
      x-api-path-slug: actioncreateuser-get
      parameters:
      - in: query
        name: Path
        description: The path for the user name
        type: string
      - in: query
        name: UserName
        description: The name of the user to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Deletes the specified IAM user.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=GetUser:
    get:
      summary: Get User
      description: |-
        Retrieves information about the specified IAM user, including the user's creation
              date, path, unique ID, and ARN.
      operationId: getUser
      x-api-path-slug: actiongetuser-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=ListUsers:
    get:
      summary: List Users
      description: Lists the IAM users that have the specified path prefix.
      operationId: listUsers
      x-api-path-slug: actionlistusers-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=PutUserPolicy:
    get:
      summary: Put User Policy
      description: |-
        Adds or updates an inline policy document that is embedded in the specified IAM
              user.
      operationId: putUserPolicy
      x-api-path-slug: actionputuserpolicy-get
      parameters:
      - in: query
        name: PolicyDocument
        description: The policy document
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document
        type: string
      - in: query
        name: UserName
        description: The name of the user to associate the policy with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users Policies
  /?Action=UpdateUser:
    get:
      summary: Update User
      description: Updates the name and/or the path of the specified IAM user.
      operationId: updateUser
      x-api-path-slug: actionupdateuser-get
      parameters:
      - in: query
        name: NewPath
        description: New path for the IAM user
        type: string
      - in: query
        name: NewUserName
        description: New name for the user
        type: string
      - in: query
        name: UserName
        description: Name of the user to update
        type: string
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