---
swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 1
info:
  title: AWS WorkDocs API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ActivateUser:
    get:
      summary: Activate User
      description: Activates the specified user.
      operationId: activateUser
      x-api-path-slug: actionactivateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=CreateUser:
    get:
      summary: Create User
      description: Creates a user in a Simple AD or Microsoft AD directory.
      operationId: createUser
      x-api-path-slug: actioncreateuser-get
      parameters:
      - in: query
        name: GivenName
        description: The given name of the user
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: Password
        description: The password of the user
        type: string
      - in: query
        name: StorageRule
        description: The amount of storage for the user
        type: string
      - in: query
        name: Surname
        description: The surname of the user
        type: string
      - in: query
        name: TimeZoneId
        description: The time zone ID of the user
        type: string
      - in: query
        name: Username
        description: The login name of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeactivateUser:
    get:
      summary: Deactivate User
      description: Deactivates the specified user, which revokes the user's access
        to Amazon WorkDocs.
      operationId: deactivateUser
      x-api-path-slug: actiondeactivateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Deletes the specified user from a Simple AD or Microsoft AD directory.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DescribeUsers:
    get:
      summary: Describe Users
      description: Describes the specified users.
      operationId: describeUsers
      x-api-path-slug: actiondescribeusers-get
      parameters:
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: Include
        description: The state of the users
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Order
        description: The order for the results
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: Query
        description: A query to filter users by user name
        type: string
      - in: query
        name: Sort
        description: The sorting criteria
        type: string
      - in: query
        name: UserIds
        description: The IDs of the users
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UpdateUser:
    get:
      summary: Update User
      description: "Updates the specified attributes of the specified user, and grants
        or revokes \n      administrative privileges to the Amazon WorkDocs site."
      operationId: updateUser
      x-api-path-slug: actionupdateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
---