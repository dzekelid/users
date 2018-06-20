---
name: Expedia
x-slug: expedia
description: Expedia Affiliate Network is the B2B partnership brand of Expedia, Inc.
  Our technology powers the hotel offering of thousands of partners around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
x-kinRank: "9"
x-alexaRank: "197733"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apis.md
specificationVersion: "0.14"
apis:
- name: Expedia (Internal Only)
  x-api-slug: expedia
  description: (Internal Only) Retrieve trip (tripId) for given customer (userId)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/users/{userId}/trips/{tripId}
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersuseridtripstripid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersuseridtripstripid-get-openapi.md
- name: Expedia (Internal Only)
  x-api-slug: expedia
  description: (Internal Only) Returns array of trips for passed userId
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/users/{userId}/trips
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersuseridtrips-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersuseridtrips-get-openapi.md
- name: Expedia User Sign-In
  x-api-slug: expedia
  description: Mobile API User Sign-In
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/user/sign-in
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersignin-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusersignin-post-openapi.md
- name: Expedia Profile
  x-api-slug: expedia
  description: Mobile API User Profile
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/user/profile
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiuserprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiuserprofile-get-openapi.md
- name: Expedia Create User
  x-api-slug: expedia
  description: Mobile API User Create
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/user/create
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusercreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiusercreate-post-openapi.md
- name: Expedia Update
  x-api-slug: expedia
  description: Mobile API User Update Traveler
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/user/update-traveler
  tags: Travel,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiuserupdatetraveler-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/apiuserupdatetraveler-post-openapi.md
- name: Expedia
  x-api-slug: expedia
  description: Expedia is the leader in travel and technology and is the worlds largest
    travel company. The EAN Developer Hub gives developers FREE access to our highly
    flexible APIs that power cutting-edge websites, mobile apps, and much more. Some
    of the best travel applications on the market are powered by the EAN API. Learn
    more reasons to partner with EAN by taking a look at our brochure and watching
    our video. The world of travel awaits you!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/expedia/openapi.md
x-common:
- type: x-base
  url: http://api.ean.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/expedia
- type: x-crunchbase
  url: https://crunchbase.com/organization/ean-upc-codes-com
- type: x-documentation
  url: https://www.expedia.com/static/mobile/swaggerui/
- type: x-email
  url: support@ean.com
- type: x-github
  url: https://github.com/Expedia
- type: x-swagger--original
  url: https://www.expedia.com/static/mobile/swaggerui/swagger.json
- type: x-twitter
  url: https://twitter.com/ExpediaEAN
- type: x-website
  url: http://developer.ean.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---