---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Get Search Users
  x-api-slug: github
  description: Search users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////search/users
  tags: Search, Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/searchusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/searchusers-get-openapi.md
- name: Github Get Users
  x-api-slug: github
  description: |-
    Get all users.
    This provides a dump of every user, in the order that they signed up for GitHub.
    Note: Pagination is powered exclusively by the since parameter. Use the Link
    header to get the URL for the next page of users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/users-get-openapi.md
- name: Github Get Users Username
  x-api-slug: github
  description: Get a single user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}
  tags: Users, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusername-get-openapi.md
- name: Github Get Users Username Events
  x-api-slug: github
  description: If you are authenticated as the given user, you will see your private
    events. Otherwise, you'll only see public events.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/events
  tags: Users, Username, Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameevents-get-openapi.md
- name: Github Get Users Username Events Orgs Org
  x-api-slug: github
  description: This is the user's organization dashboard. You must be authenticated
    as the user to view this.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/events/orgs/{org}
  tags: Users, Username, Events, Orgs, Org
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameeventsorgsorg-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameeventsorgsorg-get-openapi.md
- name: Github Get Users Username Followers
  x-api-slug: github
  description: List a user's followers
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/followers
  tags: Users, Username, Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamefollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamefollowers-get-openapi.md
- name: Github Get Users Username Following Targetuser
  x-api-slug: github
  description: Check if one user follows another.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/following/{targetUser}
  tags: Users, Username, Following, Targetuser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamefollowingtargetuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamefollowingtargetuser-get-openapi.md
- name: Github Get Users Username Gists
  x-api-slug: github
  description: List a users gists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/gists
  tags: Users, Username, Gists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamegists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamegists-get-openapi.md
- name: Github Get Users Username Keys
  x-api-slug: github
  description: |-
    List public keys for a user.
    Lists the verified public keys for a user. This is accessible by anyone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/keys
  tags: Users, Username, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamekeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamekeys-get-openapi.md
- name: Github Get Users Username Orgs
  x-api-slug: github
  description: List all public organizations for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/orgs
  tags: Users, Username, Orgs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameorgs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernameorgs-get-openapi.md
- name: Github Get Users Username Received Events
  x-api-slug: github
  description: These are events that you'll only see public events.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/received_events
  tags: Users, Username, Received, Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamereceived-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamereceived-events-get-openapi.md
- name: Github Get Users Username Received Events Public
  x-api-slug: github
  description: List public events that a user has received
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/received_events/public
  tags: Users, Username, Received, Events, Public
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamereceived-eventspublic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamereceived-eventspublic-get-openapi.md
- name: Github Get Users Username Repos
  x-api-slug: github
  description: List public repositories for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/repos
  tags: Users, Username, Repos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamerepos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamerepos-get-openapi.md
- name: Github Get Users Username Starred
  x-api-slug: github
  description: List repositories being starred by a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/starred
  tags: Users, Username, Starred
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamestarred-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamestarred-get-openapi.md
- name: Github Get Users Username Subscriptions
  x-api-slug: github
  description: List repositories being watched by a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////users/{username}/subscriptions
  tags: Users, Username, Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamesubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/usersusernamesubscriptions-get-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---