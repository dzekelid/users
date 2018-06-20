---
name: Plivo
x-slug: plivo
description: 'Voice & SMS API Platform: Plivo enables businesses and developers to
  tap into powerful Voice and SMS capabilities without carrier lock-in.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
x-kinRank: "8"
x-alexaRank: "116335"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/apis.md
specificationVersion: "0.14"
apis:
- name: Codenvy Account API Get Users
  x-api-slug: codenvy-account-api
  description: Returns the profile information for the current user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/users-get-openapi.md
- name: Codenvy Account API Get Users Followers
  x-api-slug: codenvy-account-api
  description: Returns a list of users who follow the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/:id/followers
  tags: Users,:id,Followers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/usersidfollowers-get-openapi.md
- name: Codenvy Account API Post Users Friends
  x-api-slug: codenvy-account-api
  description: Add the user to the list of followers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/:id/friends
  tags: Users,:id,Friends
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/usersidfriends-post-openapi.md
- name: Codenvy Account API Get Users Search
  x-api-slug: codenvy-account-api
  description: Return listing of ten (up to one hundred) users from search results
    for a specified search term.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/search
  tags: Users,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/userssearch-get-openapi.md
- name: Codenvy Account API Get Users Show
  x-api-slug: codenvy-account-api
  description: Returns the profile information for a specified user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/show
  tags: Users,Show
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/usersshow-get-openapi.md
- name: Codenvy Account API
  x-api-slug: codenvy-account-api
  description: 'Voice & SMS API Platform: Plivo enables businesses and developers
    to tap into powerful Voice and SMS capabilities without carrier lock-in.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/plivo/openapi.md
x-common:
- type: x--net-library
  url: https://www.plivo.com/docs/helpers/dotnet/
- type: x-android-sdk
  url: https://www.plivo.com/docs/sdk/android/
- type: x-base
  url: https://api.plivo.com
- type: x-blog
  url: http://blog.plivo.com
- type: x-blog-rss
  url: http://blog.plivo.com/rss
- type: x-crunchbase
  url: https://crunchbase.com/organization/plivo
- type: x-crunchbase
  url: http://www.crunchbase.com/company/plivo
- type: x-documentation
  url: https://plivo.com/docs/
- type: x-email
  url: marketing@plivo.com
- type: x-email
  url: legalrequests@plivo.com
- type: x-email
  url: privacy@plivo.com
- type: x-faq
  url: https://plivo.com/faq/
- type: x-github
  url: https://github.com/plivo
- type: x-ios-sdk
  url: https://www.plivo.com/docs/sdk/ios/
- type: x-java-sdk
  url: https://www.plivo.com/docs/helpers/java/
- type: x-node-js-library
  url: https://www.plivo.com/docs/helpers/node/
- type: x-php-sdk
  url: https://www.plivo.com/docs/helpers/php/
- type: x-pricing
  url: https://plivo.com/pricing/
- type: x-privacy
  url: https://plivo.com/privacy/
- type: x-ruby-library
  url: https://www.plivo.com/docs/helpers/python
- type: x-selfservice-registration
  url: https://manage.plivo.com/accounts/register/
- type: x-status
  url: https://status.plivo.com/
- type: x-terms-of-service
  url: https://plivo.com/terms/
- type: x-twitter
  url: https://twitter.com/#!/plivo
- type: x-website
  url: http:///account
- type: x-website
  url: http://plivo.com
- type: x-website
  url: https://www.plivo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---