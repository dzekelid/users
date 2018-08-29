---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Users Username
  x-api-slug: bitbucket
  description: |-
    Gets the public information associated with a user account.

    If the user's profile is private, `location`, `website` and
    `created_on` elements are omitted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}
  tags: Users, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusername-get-openapi.md
- name: Bitbucket Parameters Users Username
  x-api-slug: bitbucket
  description: Parameters users username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}
  tags: Users, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusername-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusername-parameters-openapi.md
- name: Bitbucket Get Users Username Followers
  x-api-slug: bitbucket
  description: Returns the list of accounts that are following this team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/followers
  tags: Users, Username, Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowers-get-openapi.md
- name: Bitbucket Parameters Users Username Followers
  x-api-slug: bitbucket
  description: Parameters users username followers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/followers
  tags: Users, Username, Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowers-parameters-openapi.md
- name: Bitbucket Get Users Username Following
  x-api-slug: bitbucket
  description: Returns the list of accounts this user is following.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/following
  tags: Users, Username, Following
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowing-get-openapi.md
- name: Bitbucket Parameters Users Username Following
  x-api-slug: bitbucket
  description: Parameters users username following
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/following
  tags: Users, Username, Following
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowing-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamefollowing-parameters-openapi.md
- name: Bitbucket Get Users Username Hooks
  x-api-slug: bitbucket
  description: Returns a paginated list of webhooks installed on this user account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks
  tags: Users, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-get-openapi.md
- name: Bitbucket Parameters Users Username Hooks
  x-api-slug: bitbucket
  description: Parameters users username hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks
  tags: Users, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-parameters-openapi.md
- name: Bitbucket Add Users Username Hooks
  x-api-slug: bitbucket
  description: |-
    Creates a new webhook on the specified user account.

    Account-level webhooks are fired for events from all repositories
    belonging to that account.

    Note that one can only register webhooks on one's own account, not that
    of others.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks
  tags: Users, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooks-post-openapi.md
- name: Bitbucket Delete Users Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Deletes the specified webhook subscription from the given user
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks/{uid}
  tags: Users, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-delete-openapi.md
- name: Bitbucket Get Users Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Returns the webhook with the specified id installed on the given
    user account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks/{uid}
  tags: Users, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-get-openapi.md
- name: Bitbucket Parameters Users Username Hooks U
  x-api-slug: bitbucket
  description: Parameters users username hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks/{uid}
  tags: Users, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-parameters-openapi.md
- name: Bitbucket Update Users Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/hooks/{uid}
  tags: Users, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamehooksuid-put-openapi.md
- name: Bitbucket Get Users Username Pipelines Config Variables
  x-api-slug: bitbucket
  description: Get users username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/pipelines_config/variables/
  tags: Users, Username, Pipelines, Config, Variables
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariables-get-openapi.md
- name: Bitbucket Add Users Username Pipelines Config Variables
  x-api-slug: bitbucket
  description: Post users username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/pipelines_config/variables/
  tags: Users, Username, Pipelines, Config, Variables
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariables-post-openapi.md
- name: Bitbucket Delete Users Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Delete users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/pipelines_config/variables/{variable_uuid}
  tags: Users, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket Get Users Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Get users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/pipelines_config/variables/{variable_uuid}
  tags: Users, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket Update Users Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Put users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/pipelines_config/variables/{variable_uuid}
  tags: Users, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket Get Users Username Repositories
  x-api-slug: bitbucket
  description: |-
    All repositories owned by a user/team. This includes private
    repositories, but filtered down to the ones that the calling user has
    access to.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/repositories
  tags: Users, Username, Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamerepositories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamerepositories-get-openapi.md
- name: Bitbucket Parameters Users Username Repositories
  x-api-slug: bitbucket
  description: Parameters users username repositories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//users/{username}/repositories
  tags: Users, Username, Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamerepositories-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/usersusernamerepositories-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---