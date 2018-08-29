---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework List all registrations
  description: |-
    A paginated list of registrations that the user is a contributor to. The returned registrations are sorted by their `date_modified`, with the most recently updated registrations appearing first.

    If the user ID in the path is the same as the logged-in user, all registrations will be returned. Otherwise, only the user's public registrations will be returned.

    User nodes are not available at this endpoint.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/registrations/?filter[title]=replication.

    Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
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
    patch:
      summary: Update a user
      description: |-
        Updates a user by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Users can be updated with either a **PUT** or **PATCH** request. The `full_name` field is mandatory in a **PUT** request, and optional in a **PATCH**.

        **Note**: if you make a PUT/PATCH request to the `/users/me/` endpoint, you must still provide your full user ID in the ID field of the request. We do not support using the `me` alias in request bodies at this time.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: users_partial_update
      x-api-path-slug: usersuser-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
  /users/{user_id}/addons/:
    get:
      summary: List all user addons
      description: |-
        A paginated list of authorized user addons

        #### Permissions

        User addons are visible only to the user that authorized the addon.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 addons. Each resource in the array is a separate addon object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        Attempting to request the accounts for an addon that is not enabled will result in a **404 Not Found** response.
      operationId: users_addons_list
      x-api-path-slug: usersuser-idaddons-get
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
      - Addons
  /users/{user_id}/addons/{provider}/:
    get:
      summary: Retrieve a user addon
      description: |-
        Retrieves the details of an authorized user addon

        #### Permissions

        User addons are visible only to the user that authorized the addon.

        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested user addon, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        Attempting to request the accounts for an addon that is not enabled will result in a **404 Not Found** response.
      operationId: users_addons_read
      x-api-path-slug: usersuser-idaddonsprovider-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
  /users/{user_id}/addons/{provider}/accounts/:
    get:
      summary: List all addon accounts
      description: |-
        A paginated list of addon accounts authorized by this user.

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of at most 10 addon account objects. Each resource in the array is a separate  addon account object and contains the full representation of the addon account.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: Users_addon_accounts_list
      x-api-path-slug: usersuser-idaddonsprovideraccounts-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
  /users/{user_id}/addons/{provider}/accounts/{account_id}/:
    get:
      summary: Retrieve an addon account
      description: |-
        Retrieves the details of an addon account

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested addon account, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: Users_addon_accounts_read
      x-api-path-slug: usersuser-idaddonsprovideraccountsaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: The unique identifier of the addon account
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
      - Account
  /users/{user_id}/institutions/:
    get:
      summary: List all institutions
      description: |-
        A paginated list of institutions that the user is affiliated with.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 institutions. Each resource in the array is a complete institution object and contains the full representation of the institution, meaning additional requests to a institution's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: users_institutions_list
      x-api-path-slug: usersuser-idinstitutions-get
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
      - Institutions
  /users/{user_id}/nodes/:
    get:
      summary: List all nodes
      description: |-
        A paginated list of nodes that the user is a contributor to. The returned nodes are sorted by their `date_modified`, with the most recently updated nodes appearing first.

        If the user ID in the path is the same as the logged-in user, all nodes will be returned. Otherwise, only the user's public nodes will be returned.

        User registrations are not available at this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 nodes. Each resource in the array is a separate node object and contains the full representation of the node, meaning additional requests to a node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/nodes/?filter[title]=open.

        Nodes may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, `preprint`, and `contributors`.
      operationId: users_nodes_list
      x-api-path-slug: usersuser-idnodes-get
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
      - Nodes
  /users/{user_id}/preprints/:
    get:
      summary: List all preprints
      description: |-
        A paginated list of preprints that the user contributes to. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprints. Each resource in the array is a complete preprint object and contains the full representation of the preprint, meaning additional requests to a preprint's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include preprints that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/preprints/?filter[provider]=psyarxiv.

        Preprints may be filtered by their `id`, `is_published`, `date_created`, `date_modified`, and `provider`.
      operationId: users_preprints_list
      x-api-path-slug: usersuser-idpreprints-get
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
      - Preprints
  /users/{user_id}/registrations/:
    get:
      summary: List all registrations
      description: |-
        A paginated list of registrations that the user is a contributor to. The returned registrations are sorted by their `date_modified`, with the most recently updated registrations appearing first.

        If the user ID in the path is the same as the logged-in user, all registrations will be returned. Otherwise, only the user's public registrations will be returned.

        User nodes are not available at this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/registrations/?filter[title]=replication.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: users_registrations_list
      x-api-path-slug: usersuser-idregistrations-get
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
      - Registrations
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