---
swagger: "2.0"
info:
  title: Google Doubleclick API Get User Roles
  version: 1.0.0
  description: Retrieves a list of user roles, possibly filtered. This method supports
    paging.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/userRoles:
    get:
      summary: Get User Roles
      description: Retrieves a list of user roles, possibly filtered
      operationId: dfareporting.userRoles.list
      parameters:
      - in: query
        name: accountUserRoleOnly
        description: Select only account level user roles not associated with any
          specific subaccount
      - in: query
        name: ids
        description: Select only user roles with the specified IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only user roles that belong to this subaccount
      responses:
        200:
          description: OK
      tags:
      - advertising
      - users
      - roles
definitions: []
x-collection-name: Google Doubleclick
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