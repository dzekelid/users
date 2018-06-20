---
name: AngelList
x-slug: angellist
description: AngelList is where the world meets startups. Find a great startup job,
  invest in a startup, or raise money
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
x-kinRank: "9"
x-alexaRank: "2447"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/apis.md
specificationVersion: "0.14"
apis:
- name: AngelList Get Users by Tag
  x-api-slug: angellist
  description: Get Users by Tag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///tags/{tag_id}/users
  tags: Startups,Businesses,Tags,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/tagstag-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/tagstag-idusers-get-openapi.md
- name: AngelList User Search
  x-api-slug: angellist
  description: User Search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/search
  tags: Startups,Businesses,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/userssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/userssearch-get-openapi.md
- name: AngelList Get User
  x-api-slug: angellist
  description: Get User
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/{user_id}
  tags: Startups,Businesses,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-id-get-openapi.md
- name: AngelList Get User Followers
  x-api-slug: angellist
  description: Get User Followers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/{user_id}/followers
  tags: Startups,Businesses,Users,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowers-get-openapi.md
- name: AngelList Get User Follower IDs
  x-api-slug: angellist
  description: Get User Follower IDs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/{user_id}/followers/ids
  tags: Startups,Businesses,Users,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowersids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowersids-get-openapi.md
- name: AngelList Get Users Following
  x-api-slug: angellist
  description: Get Users Following
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/{user_id}/following
  tags: Startups,Businesses,Users,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowing-get-openapi.md
- name: AngelList Get User Following IDs
  x-api-slug: angellist
  description: Get User Following IDs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///users/{user_id}/following/ids
  tags: Startups,Businesses,Users,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowingids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/usersuser-idfollowingids-get-openapi.md
- name: AngelList
  x-api-slug: angellist
  description: AngelList is where the world meets startups. Find a great startup job,
    invest in a startup, or raise money
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/angellist/openapi.md
x-common:
- type: x-blog
  url: https://blog.angel.co
- type: x-base-url
  url: http://api.angel.co/
- type: x-blog
  url: http://blog.angel.co
- type: x-blog-rss
  url: http://blog.angel.co/rss
- type: x-crunchbase
  url: http://www.crunchbase.com/company/angellist
- type: x-crunchbase
  url: https://crunchbase.com/organization/angellist
- type: x-developer
  url: https://angel.co/api
- type: x-email
  url: copyright@angel.co
- type: x-email
  url: syndicates@angel.co
- type: x-email
  url: team@angel.co
- type: x-email
  url: talent@angel.co
- type: x-email
  url: privacy@angel.co
- type: x-email
  url: abuse@angel.co
- type: x-github
  url: https://github.com/angellist
- type: x-postman-collection
  url: http://theapistack.com/data/angellist/angellist-postman-collection.json
- type: x-privacy
  url: https://angel.co/privacy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/angellist-startup-api
- type: x-support
  url: https://angel.co/help
- type: x-terms-of-service
  url: https://angel.co/terms
- type: x-twitter
  url: https://twitter.com/angellist
- type: x-website
  url: http://angel.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---