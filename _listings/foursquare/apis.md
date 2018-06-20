---
name: Foursquare
x-slug: foursquare
description: Foursquare helps you find the perfect places to go with friends. Discover
  the best food, nightlife, and entertainment in your area.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
x-kinRank: "9"
x-alexaRank: "2544"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/apis.md
specificationVersion: "0.14"
apis:
- name: Foursquare Get Users Leaderboard
  x-api-slug: foursquare
  description: /users/{USER_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/leaderboard
  tags: Users,Leaderboard
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersleaderboard-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersleaderboard-get-openapi.md
- name: Foursquare Get Users Requests
  x-api-slug: foursquare
  description: /users/leaderboard
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/requests
  tags: Users,Requests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersrequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersrequests-get-openapi.md
- name: Foursquare Get Users Search
  x-api-slug: foursquare
  description: /users/requests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/search
  tags: Users,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/userssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/userssearch-get-openapi.md
- name: Foursquare Post Users Search
  x-api-slug: foursquare
  description: users/search (GET)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/search
  tags: Users,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/userssearch-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/userssearch-post-openapi.md
- name: Foursquare Post Users Self Update
  x-api-slug: foursquare
  description: /users/{USER_ID}/unfriend
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/self/update
  tags: Users,Self
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersselfupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersselfupdate-post-openapi.md
- name: Foursquare Get Users
  x-api-slug: foursquare
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-id-get-openapi.md
- name: Foursquare Post Users Approve
  x-api-slug: foursquare
  description: /users/{USER_ID}/venuehistory
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/approve
  tags: Users,Approve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idapprove-post-openapi.md
- name: Foursquare Get Users Badges
  x-api-slug: foursquare
  description: users/search (POST)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/badges
  tags: Users,Badges
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idbadges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idbadges-get-openapi.md
- name: Foursquare Get Users Checkins
  x-api-slug: foursquare
  description: /users/{USER_ID}/badges
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/checkins
  tags: Users,Checkins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idcheckins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idcheckins-get-openapi.md
- name: Foursquare Post Users Deny
  x-api-slug: foursquare
  description: /users/{USER_ID}/approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/deny
  tags: Users,Deny
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-iddeny-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-iddeny-post-openapi.md
- name: Foursquare Get Users Friends
  x-api-slug: foursquare
  description: /users/{USER_ID}/checkins
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/friends
  tags: Users,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idfriends-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idfriends-get-openapi.md
- name: Foursquare Get Users Lists
  x-api-slug: foursquare
  description: /users/{USER_ID}/friends
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/lists
  tags: Users,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idlists-get-openapi.md
- name: Foursquare Get Users Mayorships
  x-api-slug: foursquare
  description: /users/{USER_ID}/lists
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/mayorships
  tags: Users,Mayorships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idmayorships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idmayorships-get-openapi.md
- name: Foursquare Get Users Photos
  x-api-slug: foursquare
  description: /users/{USER_ID}/mayorships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/photos
  tags: Users,Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idphotos-get-openapi.md
- name: Foursquare Post Users Request
  x-api-slug: foursquare
  description: /users/{USER_ID}/deny
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/request
  tags: Users,Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idrequest-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idrequest-post-openapi.md
- name: Foursquare Post Users Setpings
  x-api-slug: foursquare
  description: /users/{USER_ID}/request
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/setpings
  tags: Users,Setpings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idsetpings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idsetpings-post-openapi.md
- name: Foursquare Get Users Tips
  x-api-slug: foursquare
  description: /users/{USER_ID}/photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/tips
  tags: Users,Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idtips-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idtips-get-openapi.md
- name: Foursquare Get Users Todos
  x-api-slug: foursquare
  description: /users/{USER_ID}/tips
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/todos
  tags: Users,Todos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idtodos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idtodos-get-openapi.md
- name: Foursquare Post Users Unfriend
  x-api-slug: foursquare
  description: /users/{USER_ID}/setpings
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/unfriend
  tags: Users,Unfriend
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idunfriend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idunfriend-post-openapi.md
- name: Foursquare Get Users Venuehistory
  x-api-slug: foursquare
  description: /users/{USER_ID}/todos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/venuehistory
  tags: Users,Venuehistory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idvenuehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/usersuser-idvenuehistory-get-openapi.md
- name: Foursquare
  x-api-slug: foursquare
  description: foursquare makes the real world easier to use. We build tools that
    help you keep up with friends, discover whats nearby, save money and unlock deals.
    Whether youre setting off on a trip around the world, coordinating a night out
    with friends, or trying to pick out the best dish at your local restaurant, foursquare
    is the perfect companion. The foursquare API gives you access to all of the data
    used by the foursquare mobile applications, and, in some cases, even more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/foursquare/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/foursquare.json
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/foursquare/apidescription?format=internal&ver=1393644831000
- type: x-application-management
  url: https://foursquare.com/developers/apps
- type: x-blog
  url: http://engineering.foursquare.com/
- type: x-blog-rss
  url: http://engineering.foursquare.com/feed/
- type: x-curated-source
  url: http://blog.foursquare.com/2013/09/17/we-put-a-fresh-coat-of-paint-on-foursquare-for-ios-7/
- type: x-website
  url: http://blog.foursquare.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/foursquare
- type: x-crunchbase
  url: https://crunchbase.com/organization/foursquare
- type: x-email
  url: support@foursquare.com
- type: x-email
  url: ads@foursquare.com
- type: x-email
  url: press@foursquare.com
- type: x-email
  url: security@foursquare.com
- type: x-email
  url: feedback@foursquare.com
- type: x-email
  url: privacy@foursquare.com
- type: x-error-codes
  url: https://developer.foursquare.com/overview/responses
- type: x-foursquare
  url: http://foursquare.com/nasa
- type: x-foursquare
  url: http://foursquare.com/yourcommissary
- type: x-getting-started
  url: https://developer.foursquare.com/start
- type: x-github
  url: https://github.com/foursquare
- type: x-privacy
  url: https://foursquare.com/legal/privacy
- type: x-rate-limits
  url: https://developer.foursquare.com/overview/ratelimits
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/foursquare
- type: x-terms-of-service
  url: https://developer.foursquare.com/overview/community
- type: x-twitter
  url: https://twitter.com/foursquare
- type: x-twitter
  url: https://twitter.com/foursquareapi
- type: x-website
  url: http://foursquare.com
- type: x-website
  url: https://developer.foursquare.com/
- type: x-website
  url: https://foursquare.com/apps/slack
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---