---
name: Google Tasks
x-slug: google-tasks
description: The Google Tasks API lets you search, read, and update Google Tasks content
  and metadata. This document describes how to use a RESTful calling style and client
  libraries for various programming languages (currently Java, Python, and PHP) to
  access and edit Google Tasks data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/apis.md
specificationVersion: "0.14"
apis:
- name: Google Tasks API Get Users @me Lists
  x-api-slug: google-tasks-api
  description: Returns all the authenticated user's task lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists
  tags: Users, @me, Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmelists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmelists-get-openapi.md
- name: Google Tasks API Add Users @me Lists
  x-api-slug: google-tasks-api
  description: Creates a new task list and adds it to the authenticated user's task
    lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists
  tags: Users, @me, Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmelists-post-openapi.md
- name: Google Tasks API Delete Users Task List
  x-api-slug: google-tasks-api
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists/{tasklist}
  tags: Users, Task, List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Google Tasks API Get Users Task List
  x-api-slug: google-tasks-api
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists/{tasklist}
  tags: Users, Task, List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Google Tasks API Patch Users Task List
  x-api-slug: google-tasks-api
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists/{tasklist}
  tags: Users, Task, List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Google Tasks API Put Users Task List
  x-api-slug: google-tasks-api
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists/{tasklist}
  tags: Users, Task, List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Google Tasks API
  x-api-slug: google-tasks-api
  description: The Google Tasks API lets you search, read, and update Google Tasks
    content and metadata. This document describes how to use a RESTful calling style
    and client libraries for various programming languages (currently Java, Python,
    and PHP) to access and edit Google Tasks data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/google-tasks/openapi.md
x-common:
- type: x-code
  url: https://developers.google.com/google-apps/tasks/setup
- type: x-concepts
  url: https://developers.google.com/google-apps/tasks/concepts
- type: x-documentation
  url: https://developers.google.com/google-apps/tasks/v1/reference/
- type: x-website
  url: https://developers.google.com/google-apps/tasks/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---