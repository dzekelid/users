---
name: Stack Exchange
description: Stack Exchange is a network of question and answer websites on diverse
  topics in many different fields, each site covering a specific topic, where questions,
  answers, and users are subject to a reputation award process. The sites are modeled
  after Stack Overflow, a forum for computer programming questions that was the original
  site in this network. The reputation system is designed to allow the sites to be
  self-moderating.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/253_logo.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Streamrank
- Stack
- Question Answer
- Plug in
- My API Stack
- Media
- Imports
- Content
- Code
- Citations
- Answers
created: "2018-05-13"
modified: "2018-05-13"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange Get User Badges
  description: "Get the badges the users in {ids} have earned.\n \nBadge sorts are
    a tad complicated. For the purposes of sorting (and min/max) tag_based is considered
    to be greater than named.\n \nThis means that you can get a list of all tag based
    badges a user has by passing min=tag_based, and conversely all the named badges
    by passing max=named, with sort=type.\n \nFor ranks, bronze is greater than silver
    which is greater than gold. Along with sort=rank, set max=gold for just gold badges,
    max=silver&min=silver for just silver, and min=bronze for just bronze.\n \nrank
    is the default sort.\n \n{ids} can contain up to 100 semicolon delimited ids,
    to find ids programatically look for user_id on user or shallow_user objects.\n
    \nThis method returns a list of badges."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/253_logo.png
  humanURL: https://stackexchange.com/
  baseURL: https://api.stackexchange.com//2.2
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-ids-badges-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-ids-badges-get-postman.md
- name: Stack Exchange Get User Notifications
  description: "Returns a user's notifications.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of notifications."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/253_logo.png
  humanURL: https://stackexchange.com/
  baseURL: https://api.stackexchange.com//2.2
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-id-notifications-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-id-notifications-get-postman.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: https://stackexchange.com/
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---