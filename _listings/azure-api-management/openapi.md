---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users
  : get:
      summary: GroupUsers ListByGroups
      description: Lists a collection of the members of the group, specified by its
        identifier.
      operationId: GroupUsers_ListByGroups
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusers-get
      parameters:
      - in: query
        name: $filter
        description: '| Field            | Supported operators    | Supported functions               ||------------------|------------------------|-----------------------------------||
          id               | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || firstName        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || lastName         | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || email            | ge, le, eq, ne, gt,
          lt | substringof, contains, startswith, endswith || state            | eq                     |
          N/A                               || registrationDate | ge, le, eq, ne,
          gt, lt | N/A                               || note             | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users/{uid}
  : put:
      summary: GroupUsers Create
      description: Adds a user to the specified group.
      operationId: GroupUsers_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
    delete:
      summary: GroupUsers Delete
      description: Remove existing user from existing group.
      operationId: GroupUsers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users:
    get:
      summary: Users ListByService
      description: Lists a collection of registered users in the specified service
        instance.
      operationId: Users_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusers-get
      parameters:
      - in: query
        name: $filter
        description: '| Field            | Supported operators    | Supported functions               ||------------------|------------------------|-----------------------------------||
          id               | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || firstName        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || lastName         | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || email            | ge, le, eq, ne, gt,
          lt | substringof, contains, startswith, endswith || state            | eq                     |
          N/A                               || registrationDate | ge, le, eq, ne,
          gt, lt | N/A                               || note             | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  : get:
      summary: Users Get
      description: Gets the details of the user specified by its identifier.
      operationId: Users_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
    put:
      summary: Users CreateOrUpdate
      description: Creates or Updates a user.
      operationId: Users_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create or update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Users Update
      description: Updates the details of the user specified by its identifier.
      operationId: Users_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-patch
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the user to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
    delete:
      summary: Users Delete
      description: Deletes specific user.
      operationId: Users_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-delete
      parameters:
      - in: query
        name: deleteSubscriptions
        description: Whether to delete users subscription or not
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the user to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/generateSsoUrl
  : post:
      summary: Users GenerateSsoUrl
      description: Retrieves a redirection URL containing an authentication token
        for signing a given user into the developer portal.
      operationId: Users_GenerateSsoUrl
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgeneratessourl-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/groups
  : get:
      summary: UserGroups ListByUsers
      description: Lists all user groups.
      operationId: UserGroups_ListByUsers
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidgroups-get
      parameters:
      - in: query
        name: $filter
        description: '| Field       | Supported operators    | Supported functions                         ||-------------|------------------------|---------------------------------------------||
          id          | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || name        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || description | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/subscriptions
  : get:
      summary: UserSubscriptions ListByUsers
      description: Lists the collection of subscriptions of the specified user.
      operationId: UserSubscriptions_ListByUsers
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuidsubscriptions-get
      parameters:
      - in: query
        name: $filter
        description: '| Field        | Supported operators    | Supported functions                         ||--------------|------------------------|---------------------------------------------||
          id           | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || name         | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || stateComment | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || userId       | ge, le, eq, ne, gt, lt
          | substringof, contains, startswith, endswith || productId    | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith || state        |
          eq                     |                                             |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}/identities
  : get:
      summary: UserIdentities ListByUsers
      description: Lists all user identities.
      operationId: UserIdentities_ListByUsers
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuididentities-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
---