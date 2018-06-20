---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "443"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box Create User
  x-api-slug: box
  description: Used to provision a new user in an enterprise. This method only works
    for enterprise admins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users
  tags: Documents,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/users-post-openapi.md
- name: Box Get Enterprise Users
  x-api-slug: box
  description: Returns a list of all users for the Enterprise along with their user_id,
    public_name, and login.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users
  tags: Documents,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/users-get-openapi.md
- name: Box Get Current User
  x-api-slug: box
  description: Retrieves information about the user who is currently logged in i.e.
    the user for whom this auth token was generated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/me
  tags: Documents,Users, Me
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersme-get-openapi.md
- name: Box Get User's Info
  x-api-slug: box
  description: Retrieves information about a user in the enterprise. Requires enterprise
    administration authorization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}
  tags: Documents,Users, User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-id-get-openapi.md
- name: Box Update User, Change User's Login
  x-api-slug: box
  description: "Used to edit the settings and information about a user. This method
    only works for enterprise admins. To roll a user out of the enterprise (and convert
    them to a standalone free user), update the special enterprise attribute to be
    null.\n\nUsed to convert one of the user\u2019s confirmed email aliases into the
    user\u2019s primary login."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}
  tags: Documents,Users, User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-id-put-openapi.md
- name: Box Delete User
  x-api-slug: box
  description: Deletes a user in an enterprise account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}
  tags: Documents,Users, User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-id-delete-openapi.md
- name: Box Move User's Folder
  x-api-slug: box
  description: "Moves all of the owned content from within one user\u2019s folder
    into a new folder in another user\u2019s account. You can move folders across
    users as long as the you have administrative permissions and the \u2018source\u2019
    user owns the folders. To move everything from the root folder, use \u201C0\u201D
    which always represents the root folder of a Box account."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}/folders/{FOLDER_ID}
  tags: Documents,Users, User, , Folders, Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idfoldersfolder-id-put-openapi.md
- name: Box Get Email Aliases
  x-api-slug: box
  description: Retrieves all email aliases for this user. The collection of email
    aliases does not include the primary login for the user; use GET /users/USER_ID
    to retrieve the login email address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}/email_aliases
  tags: Documents,Users, User, , Email, Aliases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idemail-aliases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idemail-aliases-get-openapi.md
- name: Box Add Email Alias
  x-api-slug: box
  description: "Adds a new email alias to the given user\u2019s account."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}/email_aliases
  tags: Documents,Users, User, , Email, Aliases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idemail-aliases-post-openapi.md
- name: Box Delete Email Alias
  x-api-slug: box
  description: Removes an email alias from a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}/email_aliases/{EMAIL_ALIAS_ID}
  tags: Documents,Users, User, , Email, Aliases, Email, Alias
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idemail-aliasesemail-alias-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idemail-aliasesemail-alias-id-delete-openapi.md
- name: Box Get Memberships for User
  x-api-slug: box
  description: Retrieves all of the group memberships for a given user. Note this
    is only available to group admins. To retrieve group memberships for the user
    making the API request, use the users/me/memberships endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//users/{USER_ID}/memberships
  tags: Documents,Users, User, , Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/usersuser-idmemberships-get-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---