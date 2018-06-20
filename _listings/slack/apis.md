---
name: Slack
x-slug: slack
description: Slack is a team communication application providing services such as
  real-time messaging, archiving, and to search for modern teams. It offers one-on-one
  messaging, private groups, persistent chat rooms, and direct messaging as well as
  group chats organized by topic. All content inside Slack is searchable from one
  search box and it integrates with a number of third-party services, including Google
  Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/apis.md
specificationVersion: "0.14"
apis:
- name: Slack Set User Profile
  x-api-slug: slack
  description: Set the profile information for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.profile.set
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-profile-set-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-profile-set-post-openapi.md
- name: Slack Set User Presence
  x-api-slug: slack
  description: Manually sets user presence.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.setPresence
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setpresence-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setpresence-post-openapi.md
- name: Slack Get User Info
  x-api-slug: slack
  description: Gets information about a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.info
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-info-get-openapi.md
- name: Slack Find User
  x-api-slug: slack
  description: Find a user with an email address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.lookupByEmail
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-lookupbyemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-lookupbyemail-get-openapi.md
- name: Slack Set User Profile Photo
  x-api-slug: slack
  description: Set the user profile photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.setPhoto
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setphoto-post-openapi.md
- name: Slack Get User Identity
  x-api-slug: slack
  description: Get a user's identity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.identity
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-identity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-identity-get-openapi.md
- name: Slack Get User Profile
  x-api-slug: slack
  description: Retrieves a user's profile information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.profile.get
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-profile-get-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-profile-get-get-openapi.md
- name: Slack List Team Users
  x-api-slug: slack
  description: Lists all users in a Slack team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.list
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-list-get-openapi.md
- name: Slack Make User Inactive
  x-api-slug: slack
  description: Marks a user as active.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//users.setActive
  tags: Messaging,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setactive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/users-setactive-post-openapi.md
- name: Slack
  x-api-slug: slack
  description: Slack is a team communication application providing services such as
    real-time messaging, archiving, and to search for modern teams. It offers one-on-one
    messaging, private groups, persistent chat rooms, and direct messaging as well
    as group chats organized by topic. All content inside Slack is searchable from
    one search box and it integrates with a number of third-party services, including
    Google Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/slack/openapi.md
x-common:
- type: x-website
  url: https://api.slack.com
- type: x-application-gallery
  url: https://slack.com/apps
- type: x-blog
  url: http://slackhq.com/
- type: x-blog
  url: https://medium.com/slack-developer-blog
- type: x-blog-rss
  url: http://slackhq.com/rss
- type: x-blog-rss
  url: https://medium.com/feed/slack-developer-blog
- type: x-branding
  url: https://slack.com/brand-guidelines
- type: x-buttons
  url: https://api.slack.com/docs/slack-button
- type: x-c-sharp-sdk
  url: https://api.slack.com/web
- type: x-change-log
  url: https://api.slack.com/changelog
- type: x-developer
  url: https://api.slack.com/
- type: x-faq
  url: https://api.slack.com/faq
- type: x-getting-started
  url: https://slack.com/getting-started
- type: x-github
  url: https://github.com/slackhq
- type: x-incoming-webhooks
  url: https://api.slack.com/incoming-webhooks
- type: x-oauth-overview
  url: https://api.slack.com/docs/oauth
- type: x-oauth-scopes
  url: https://api.slack.com/docs/oauth-scopes
- type: x-outgoing-webhooks
  url: https://api.slack.com/outgoing-webhooks
- type: x-presence
  url: https://api.slack.com/docs/presence
- type: x-pricing
  url: https://slack.com/pricing
- type: x-privacy
  url: https://slack.com/privacy-policy
- type: x-rate-limits
  url: https://api.slack.com/docs/rate-limits
- type: x-real-time-messaging-api
  url: https://api.slack.com/rtm
- type: x-road-map
  url: https://api.slack.com/roadmap
- type: x-security
  url: https://slack.com/security
- type: x-status
  url: https://status.slack.com/
- type: x-support
  url: https://get.slack.help/hc/en-us
- type: x-terms-of-service
  url: https://slack.com/terms-of-service
- type: x-transparency-report
  url: https://slack.com/transparency-report
- type: x-twitter
  url: https://twitter.com/slackapi
- type: x-website
  url: http://slack.com
- type: x-website
  url: https://slack.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---