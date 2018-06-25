---
name: Learnifier
x-slug: learnifier
description: Create your online courses in minutes. Learnifier is the fast and easy
  tool for creating and sharing great courses that work on your mobile, tablet and
  desktop. Book a DEMO or test it out with our FREE TRIAL.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
x-kinRank: "7"
x-alexaRank: "5836977"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/apis.md
specificationVersion: "0.14"
apis:
- name: Learnifier Gets a user by external id
  x-api-slug: learnifier
  description: Gets a user by external id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////extuser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/extuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/extuser-get-openapi.md
- name: Learnifier List Global User Groups.
  x-api-slug: learnifier
  description: Returns a list of Global User Groups. Global User Groups are set up
    for the realm, and will generate groups that can be used on the client level.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////globalusergroups
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/globalusergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/globalusergroups-get-openapi.md
- name: Learnifier List of all users in group.
  x-api-slug: learnifier
  description: Returns a list of all members in User Groups that are based on the
    Global Group with this groupid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////globalusergroups/{groupid}/members
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/globalusergroupsgroupidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/globalusergroupsgroupidmembers-get-openapi.md
- name: Learnifier List User Groups.
  x-api-slug: learnifier
  description: Returns a list of User Groups for the org unit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups
  tags: Organizations,Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/orgunitsorgidusergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/orgunitsorgidusergroups-get-openapi.md
- name: Learnifier Create a User Group.
  x-api-slug: learnifier
  description: Create a User Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups
  tags: Organizations,Users,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/orgunitsorgidusergroups-post-openapi.md
- name: Learnifier Get user group
  x-api-slug: learnifier
  description: Returns single User Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups/{groupid}
  tags: Organizations,Users,Groups,Groupid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/orgunitsorgidusergroupsgroupid-get-openapi.md
- name: Learnifier Lists all users
  x-api-slug: learnifier
  description: Lists all users. Only api callers that have full access can call this
    method.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/users-get-openapi.md
- name: Learnifier Adds a user
  x-api-slug: learnifier
  description: Adds a user. No two users can have the same email address. Email is
    saved WITH case but compared regardless of case. Email can be changed for a user
    assuming it doesn't cause a conflict.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/users-post-openapi.md
- name: Learnifier User information
  x-api-slug: learnifier
  description: Returns information about a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users/{userid}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/usersuserid-get-openapi.md
- name: Learnifier Updates user information
  x-api-slug: learnifier
  description: Updates a user. All values that have a key defined in the input will
    be set. So if a value should not be updated omit it totally from the input, otherwise
    it will be unset.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users/{userid}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/usersuserid-patch-openapi.md
- name: Learnifier User profile picture
  x-api-slug: learnifier
  description: |-
    Returns a thumbnail picture of the user. This can either be a selected picture or an auto generated image. This method doesn't require a full sign in. The api key is sufficient.
    The image is square and is likely, but not necessary, to be in 128x128 PNG format. However the format will always be either PNG, JPEG or GIF.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users/{userid}/pic?key={APIKEY}
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/usersuseridpickeyapikey-get-openapi.md
- name: Learnifier Returns information about the projects the user is a participant
    in.
  x-api-slug: learnifier
  description: Returns information about the projects the user is a participant in.
    Only the projects that the current token have access to will be listed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////users/{userid}/projectParticipations
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/usersuseridprojectparticipations-get-openapi.md
- name: Learnifier
  x-api-slug: learnifier
  description: Create your online courses in minutes. Learnifier is the fast and easy
    tool for creating and sharing great courses that work on your mobile, tablet and
    desktop. Book a DEMO or test it out with our FREE TRIAL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/learnifier/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/learnifier
- type: x-developer
  url: https://learnifier.com/api/
- type: x-email
  url: sales@learnifier.com
- type: x-email
  url: Abdalla.Mohamed@learnifier.com
- type: x-email
  url: support@learnifier.com
- type: x-email
  url: jerker.klang@learnifier.com
- type: x-email
  url: mattias.borg@learnifier.com
- type: x-email
  url: lars.peterstrand@learnifier.com
- type: x-email
  url: hello@learnifier.com
- type: x-email
  url: unsubscribe@learnifier.com
- type: x-email
  url: privacy@learnifier.com
- type: x-twitter
  url: https://twitter.com/Learnifier
- type: x-website
  url: http://learnifier.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---