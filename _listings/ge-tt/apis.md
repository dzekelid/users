---
name: Ge.tt
x-slug: ge-tt
description: Extremely simple realtime filesharing. No signup required. Share any
  number of photos, videos, music, anything - in seconds - no matter how large.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1012-ge-tt.jpg
x-kinRank: "8"
x-alexaRank: "36546"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/apis.md
specificationVersion: "0.14"
apis:
- name: Ge.tt  REST API Users Login
  x-api-slug: ge-tt--rest-api
  description: 'The API is based on oauth with an xauth handshake. The request body
    looks like this:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1012-ge-tt.jpg
  humanURL: http://ge.tt
  baseURL: https://open.ge.tt//1//1/users/login
  tags: Users,Login
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/1userslogin-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/1userslogin-post-openapi.md
- name: Ge.tt  REST API Users Me
  x-api-slug: ge-tt--rest-api
  description: 'Returns your user information:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1012-ge-tt.jpg
  humanURL: http://ge.tt
  baseURL: https://open.ge.tt//1//1/users/me
  tags: Users,Me
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/1usersme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/1usersme-get-openapi.md
- name: Ge.tt  REST API
  x-api-slug: ge-tt--rest-api
  description: The Ge.tt API allows you to use Ge.tt in your own applications. We
    believe that our users should be able to access their files and share their content
    in their platform of choice. By using the API, developers are able to easily put
    their own content, or the content of their users online. At the same time they
    are able to use Ge.tts unique real-time file sharing technology where files are
    available before they are even uploaded.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1012-ge-tt.jpg
  humanURL: http://ge.tt
  baseURL: https://open.ge.tt//1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/ge-tt/openapi.md
x-common:
- type: x--net-library
  url: http://ge.tt/developers/csharp
- type: x-base
  url: http://open.ge.tt
- type: x-blog
  url: http://ge.tt/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/ge-tt
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://ge.tt/developers
- type: x-email
  url: hello@ge.tt
- type: x-facebook
  url: https://www.facebook.com/gettsharing
- type: x-faq
  url: http://ge.tt/faq
- type: x-getting-started
  url: http://ge.tt/developers/start
- type: x-github
  url: https://github.com/gett
- type: x-java-library
  url: http://ge.tt/developers/java
- type: x-perl-library
  url: http://ge.tt/developers/perl
- type: x-python-library
  url: http://ge.tt/developers/python
- type: x-terms-of-service
  url: http://ge.tt/terms
- type: x-twitter
  url: https://twitter.com/gettsharing
- type: x-website
  url: http://ge.tt
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---