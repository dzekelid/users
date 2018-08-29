---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Get users
  x-api-slug: mattermost-api
  description: |-
    Get a page of a list of users. Based on query string parameters, select users from a team, channel, or select users not in a specific channel.

    Since server version 4.0, some basic sorting is available using the `sort` query parameter. Sorting is currently only supported when selecting users on a team.
    ##### Permissions
    Requires an active session and (if specified) membership to the channel or team being selected from.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/users-get-openapi.md
- name: Mattermost API Get users by ids
  x-api-slug: mattermost-api
  description: |-
    Get a list of users based on a provided list of user ids.
    ##### Permissions
    Requires an active session but no other permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/ids
  tags: Users,By,Ids
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersids-post-openapi.md
- name: Mattermost API Get users by usernames
  x-api-slug: mattermost-api
  description: |-
    Get a list of users based on a provided list of usernames.
    ##### Permissions
    Requires an active session but no other permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/usernames
  tags: Users,By,Usernames
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersusernames-post-openapi.md
- name: Mattermost API Search users
  x-api-slug: mattermost-api
  description: |-
    Get a list of users based on search criteria provided in the request body. Searches are typically done against username, full name, nickname and email unless otherwise configured by the server.
    ##### Permissions
    Requires an active session and `read_channel` and/or `view_team` permissions for any channels or teams specified in the request body.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/search
  tags: Search,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/userssearch-post-openapi.md
- name: Mattermost API Autocomplete users
  x-api-slug: mattermost-api
  description: |-
    Get a list of users for the purpose of autocompleting based on the provided search term. Specify a combination of `team_id` and `channel_id` to filter results further.
    ##### Permissions
    Requires an active session and `view_team` and `read_channel` on any teams or channels used to filter the results further.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/autocomplete
  tags: Autocomplete,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersautocomplete-get-openapi.md
- name: Mattermost API Update a user's roles
  x-api-slug: mattermost-api
  description: |-
    Update a user's system-level roles. Valid user roles are "system_user", "system_admin" or both of them. Overwrites any previously assigned system-level roles.
    ##### Permissions
    Must have the `manage_roles` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/roles
  tags: Users,Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idroles-put-openapi.md
- name: Mattermost API Get user's profile image
  x-api-slug: mattermost-api
  description: |-
    Get a user's profile image based on user_id string parameter.
    ##### Permissions
    Must be logged in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/image
  tags: Users,Profile,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idimage-get-openapi.md
- name: Mattermost API Set user's profile image
  x-api-slug: mattermost-api
  description: |-
    Set a user's profile image based on user_id string parameter.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/image
  tags: Set,Users,Profile,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idimage-post-openapi.md
- name: Mattermost API Update a user's MFA
  x-api-slug: mattermost-api
  description: |-
    Activates multi-factor authentication for the user if `activate` is true and a valid `code` is provided. If activate is false, then `code` is not required and multi-factor authentication is disabled for the user.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/mfa
  tags: Users,MFA
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idmfa-put-openapi.md
- name: Mattermost API Update a user's password
  x-api-slug: mattermost-api
  description: |-
    Update a user's password. New password must meet password policy set by server configuration. Current password is required if you're updating your own password.
    ##### Permissions
    Must be logged in as the user the password is being changed for or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/password
  tags: Users,Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idpassword-put-openapi.md
- name: Mattermost API Get user's sessions
  x-api-slug: mattermost-api
  description: |-
    Get a list of sessions by providing the user GUID. Sensitive information will be sanitized out.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/sessions
  tags: Users,Sessions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idsessions-get-openapi.md
- name: Mattermost API Get users audits
  x-api-slug: mattermost-api
  description: |-
    Get a list of audit by providing the user GUID.
    ##### Permissions
    Must be logged in as the user or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/audits
  tags: Users,Audits
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idaudits-get-openapi.md
- name: Mattermost API Update a users authentication method
  x-api-slug: mattermost-api
  description: |-
    Updates a user's authentication method. This can be used to change them to/from LDAP authentication for example.

    __Minimum server version__: 4.6
    ##### Permissions
    Must have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/auth
  tags: Users,Authentication,Method
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idauth-put-openapi.md
- name: Mattermost API Get a user's teams
  x-api-slug: mattermost-api
  description: |-
    Get a list of teams that a user is on.
    ##### Permissions
    Must be authenticated as the user or have the `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/teams
  tags: Users,Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idteams-get-openapi.md
- name: Mattermost API Add multiple users to team
  x-api-slug: mattermost-api
  description: |-
    Add a number of users to the team by user_id.
    ##### Permissions
    Must be authenticated. Authenticated user must have the `add_user_to_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/members/batch
  tags: Multiple,Users,To,Team
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/teamsteam-idmembersbatch-post-openapi.md
- name: Mattermost API Invite users to the team by email
  x-api-slug: mattermost-api
  description: |-
    Invite users to the existing team usign the user's email.
    ##### Permissions
    Must have `invite_to_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/invite/email
  tags: Invite,Users,To,Team,By,Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/teamsteam-idinviteemail-post-openapi.md
- name: Mattermost API Get the user's preferences
  x-api-slug: mattermost-api
  description: |-
    Get a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences
  tags: Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idpreferences-get-openapi.md
- name: Mattermost API Save the user's preferences
  x-api-slug: mattermost-api
  description: |-
    Save a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences
  tags: Save,Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idpreferences-put-openapi.md
- name: Mattermost API Delete user's preferences
  x-api-slug: mattermost-api
  description: |-
    Delete a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences/delete
  tags: Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idpreferencesdelete-post-openapi.md
- name: Mattermost API List a user's preferences by category
  x-api-slug: mattermost-api
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences/{category}
  tags: List,Users,Preferences,By,Category
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API
  x-api-slug: mattermost-api
  description: Open source, private cloud Slack-alternative, Workplace messaging for
    web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
    configurable, and scalable from teams to the enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/mattermost/openapi.md
x-common:
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---