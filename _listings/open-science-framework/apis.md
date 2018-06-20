---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework List all affiliated users
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//institutions/{institution_id}/users/
  tags: Institutions,Institution,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/institutionsinstitution-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/institutionsinstitution-idusers-get-openapi.md
- name: Open Science Framework List all users
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/users-get-openapi.md
- name: Open Science Framework Retrieve a user
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a given users.

    The returned information includes the user's bibliographic information and the date the user was registered.

    Additionally, relationships to the list of institutions with which the user is affiliated, and to the list of nodes which the user contributes to (that the requesting user has permission to see) are returned.

    If `me` is given as the `user_id` in the request path, the record of the currently logged-in user will be returned.
    #### Returns
    Returns a JSON object with a `data` key containing the representation of the requested user, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/
  tags: Users,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-id-get-openapi.md
- name: Open Science Framework Update a user
  x-api-slug: open-science-framework
  description: |-
    Updates a user by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

    Users can be updated with either a **PUT** or **PATCH** request. The `full_name` field is mandatory in a **PUT** request, and optional in a **PATCH**.

    **Note**: if you make a PUT/PATCH request to the `/users/me/` endpoint, you must still provide your full user ID in the ID field of the request. We do not support using the `me` alias in request bodies at this time.
    #### Returns
    Returns a JSON object with a `data` key containing the new representation of the updated node, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/
  tags: Users,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-id-patch-openapi.md
- name: Open Science Framework List all user addons
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/addons/
  tags: Users,User,Addons
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddons-get-openapi.md
- name: Open Science Framework Retrieve a user addon
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of an authorized user addon

    #### Permissions

    User addons are visible only to the user that authorized the addon.

    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested user addon, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

    Attempting to request the accounts for an addon that is not enabled will result in a **404 Not Found** response.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/addons/{provider}/
  tags: Users,User,Addons,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddonsprovider-get-openapi.md
- name: Open Science Framework List all addon accounts
  x-api-slug: open-science-framework
  description: |-
    A paginated list of addon accounts authorized by this user.

    #### Permissions

    Addon accounts are visible only to the user that authorized the account.

    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of at most 10 addon account objects. Each resource in the array is a separate  addon account object and contains the full representation of the addon account.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/addons/{provider}/accounts/
  tags: Users,User,Addons,Provider,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddonsprovideraccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddonsprovideraccounts-get-openapi.md
- name: Open Science Framework Retrieve an addon account
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of an addon account

    #### Permissions

    Addon accounts are visible only to the user that authorized the account.

    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested addon account, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/addons/{provider}/accounts/{account_id}/
  tags: Users,User,Addons,Provider,Accounts,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddonsprovideraccountsaccount-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idaddonsprovideraccountsaccount-id-get-openapi.md
- name: Open Science Framework List all institutions
  x-api-slug: open-science-framework
  description: |-
    A paginated list of institutions that the user is affiliated with.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 institutions. Each resource in the array is a complete institution object and contains the full representation of the institution, meaning additional requests to a institution's detail view are not necessary.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/institutions/
  tags: Users,User,Institutions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idinstitutions-get-openapi.md
- name: Open Science Framework List all nodes
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/nodes/
  tags: Users,User,Nodes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idnodes-get-openapi.md
- name: Open Science Framework List all preprints
  x-api-slug: open-science-framework
  description: |-
    A paginated list of preprints that the user contributes to. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 preprints. Each resource in the array is a complete preprint object and contains the full representation of the preprint, meaning additional requests to a preprint's detail view are not necessary.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include preprints that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/preprints/?filter[provider]=psyarxiv.

    Preprints may be filtered by their `id`, `is_published`, `date_created`, `date_modified`, and `provider`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/preprints/
  tags: Users,User,Preprints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idpreprints-get-openapi.md
- name: Open Science Framework List all registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/registrations/
  tags: Users,User,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/usersuser-idregistrations-get-openapi.md
- name: Open Science Framework
  x-api-slug: open-science-framework
  description: OSF provides free and open source project management support for researchers
    across the entire research lifecycle. As a collaboration tool, OSF helps researchers
    work on projects privately with a limited number of collaborators and make parts
    of their projects public, or make all the project publicly accessible for broader
    dissemination. As a workflow system, OSF enables connections to the many services
    researchers already use to streamline their process and increase efficiency. As
    a flexible repository, it can store and archive research data, protocols, and
    materials.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/open-science-framework/openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---