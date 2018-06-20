---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework Retrieve a user
  description: |-
    Retrieves the details of a given users.

    The returned information includes the user's bibliographic information and the date the user was registered.

    Additionally, relationships to the list of institutions with which the user is affiliated, and to the list of nodes which the user contributes to (that the requesting user has permission to see) are returned.

    If `me` is given as the `user_id` in the request path, the record of the currently logged-in user will be returned.
    #### Returns
    Returns a JSON object with a `data` key containing the representation of the requested user, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /institutions/{institution_id}/users/:
    get:
      summary: List all affiliated users
      description: |-
        A paginated list of all users affiliated with an institution.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 users. Each resource in the array is a separate users object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        You can optionally request that the response only include users that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/cos/users?filter[family_name]=Nosek.

        Users may be filtered by their `id`, `full_name`, `given_name`, `middle_names`, and `family_name`
      operationId: institutions_users_list
      x-api-path-slug: institutionsinstitution-idusers-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
      - Users
  /users/:
    get:
      summary: List all users
      description: |-
        A paginated list of all users registered on the OSF. The returned users are sorted by their `date_registered`, with the most recently registered users appearing first.

        The subroute `/users/me/` is a special endpoint that always points to the currently logged-in user.
        #### Versioning
        As of version `2.3`, merged users will not be returned from this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 users. Each resource in the array is a separate users object and contains the full representation of the user, meaning additional requests to a user's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/?filter[family_name]=Nosek.

        Users may be filtered by their `id`, `full_name`, `given_name`, `middle_name`, or `family_name`.
      operationId: users_list
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/:
    get:
      summary: Retrieve a user
      description: |-
        Retrieves the details of a given users.

        The returned information includes the user's bibliographic information and the date the user was registered.

        Additionally, relationships to the list of institutions with which the user is affiliated, and to the list of nodes which the user contributes to (that the requesting user has permission to see) are returned.

        If `me` is given as the `user_id` in the request path, the record of the currently logged-in user will be returned.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested user, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: users_read
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
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