---
name: SoundCloud
x-slug: soundcloud
description: SoundCloud is a music and podcast streaming platform that lets you listen
  to millions of songs from around the world, or upload your own. Start listening
  now!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
x-kinRank: "9"
x-alexaRank: "112"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/apis.md
specificationVersion: "0.14"
apis:
- name: Sound Cloud Get Users
  x-api-slug: sound-cloud
  description: Returns a collection of users
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users.json
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/users-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/users-json-get-openapi.md
- name: Sound Cloud Get Users
  x-api-slug: sound-cloud
  description: Returns a user by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}.json
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-id-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-id-json-get-openapi.md
- name: Sound Cloud Get Users Tracks
  x-api-slug: sound-cloud
  description: Returns a collection of tracks uploaded by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/tracks.json
  tags: Users,Tracks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idtracks-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idtracks-json-get-openapi.md
- name: Sound Cloud Get Users Comments
  x-api-slug: sound-cloud
  description: Returns a collection of comments made by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/comments.json
  tags: Users,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idcomments-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idcomments-json-get-openapi.md
- name: Sound Cloud Get Users Followings
  x-api-slug: sound-cloud
  description: Returns a collection of users the user with user id is following
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings.json
  tags: Users,Followings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowings-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowings-json-get-openapi.md
- name: Sound Cloud Get Users Followings Contact
  x-api-slug: sound-cloud
  description: Checks if the user with the id contact_id is in the givens user's list
    of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.json
  tags: Users,Followings,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-get-openapi.md
- name: Sound Cloud Put Users Followings Contact
  x-api-slug: sound-cloud
  description: Adds the user with the id contact_id to the givens user's list of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.json
  tags: Users,Followings,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-put-openapi.md
- name: Sound Cloud Delete Users Followings Contact
  x-api-slug: sound-cloud
  description: Removes the user with the id contact_id from the givens user's list
    of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.json
  tags: Users,Followings,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-json-delete-openapi.md
- name: Sound Cloud Get Users Followers
  x-api-slug: sound-cloud
  description: Returns a collection of users who follow the user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followers.json
  tags: Users,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowers-json-get-openapi.md
- name: Sound Cloud Get Users Followers Contact
  x-api-slug: sound-cloud
  description: Checks if the user with contact_id is a follower of the given user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followers/{contact_id}.json
  tags: Users,Followers,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowerscontact-id-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowerscontact-id-json-get-openapi.md
- name: Sound Cloud Get Users Favorites
  x-api-slug: sound-cloud
  description: Returns a collection of tracks favorited by the user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites.json
  tags: Users,Favorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavorites-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavorites-json-get-openapi.md
- name: Sound Cloud Put Users Favorites Track
  x-api-slug: sound-cloud
  description: Adds the given track to the given user's list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites/{track_id}.json
  tags: Users,Favorites,Track
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-json-put-openapi.md
- name: Sound Cloud Delete Users Favorites Track
  x-api-slug: sound-cloud
  description: Deletes the given track from the given user's list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites/{track_id}.json
  tags: Users,Favorites,Track
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-json-delete-openapi.md
- name: Sound Cloud Get Users Groups
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/groups.json
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idgroups-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idgroups-json-get-openapi.md
- name: Sound Cloud Get Users Playlists
  x-api-slug: sound-cloud
  description: Returns a collection of playlists created by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/playlists.json
  tags: Users,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idplaylists-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idplaylists-json-get-openapi.md
- name: Sound Cloud Get Groups Users
  x-api-slug: sound-cloud
  description: Returns a combined collection of moderators, members and contributors
    of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/users.json
  tags: Groups,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/groupsgroup-idusers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/groupsgroup-idusers-json-get-openapi.md
- name: Sound Cloud Get Users. Format
  x-api-slug: sound-cloud
  description: Returns a collection of users
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users.{format}
  tags: Users,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/users-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/users-format-get-openapi.md
- name: Sound Cloud Get Users . Format
  x-api-slug: sound-cloud
  description: Returns a user by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}.{format}
  tags: Users,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-id-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-id-format-get-openapi.md
- name: Sound Cloud Get Users Tracks. Format
  x-api-slug: sound-cloud
  description: Returns a collection of tracks uploaded by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/tracks.{format}
  tags: Users,Tracks,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idtracks-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idtracks-format-get-openapi.md
- name: Sound Cloud Get Users Comments. Format
  x-api-slug: sound-cloud
  description: Returns a collection of comments made by user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/comments.{format}
  tags: Users,Comments,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idcomments-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idcomments-format-get-openapi.md
- name: Sound Cloud Get Users Followings. Format
  x-api-slug: sound-cloud
  description: Returns a collection of users the user with user id is following
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings.{format}
  tags: Users,Followings,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowings-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowings-format-get-openapi.md
- name: Sound Cloud Get Users Followings Contact . Format
  x-api-slug: sound-cloud
  description: Checks if the user with the id contact_id is in the givens user's list
    of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.{format}
  tags: Users,Followings,Contact,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-get-openapi.md
- name: Sound Cloud Put Users Followings Contact . Format
  x-api-slug: sound-cloud
  description: Adds the user with the id contact_id to the givens user's list of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.{format}
  tags: Users,Followings,Contact,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-put-openapi.md
- name: Sound Cloud Delete Users Followings Contact . Format
  x-api-slug: sound-cloud
  description: Removes the user with the id contact_id from the givens user's list
    of contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followings/{contact_id}.{format}
  tags: Users,Followings,Contact,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowingscontact-id-format-delete-openapi.md
- name: Sound Cloud Get Users Followers. Format
  x-api-slug: sound-cloud
  description: Returns a collection of users who follow the user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followers.{format}
  tags: Users,Followers,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowers-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowers-format-get-openapi.md
- name: Sound Cloud Get Users Followers Contact . Format
  x-api-slug: sound-cloud
  description: Checks if the user with contact_id is a follower of the given user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/followers/{contact_id}.{format}
  tags: Users,Followers,Contact,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowerscontact-id-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfollowerscontact-id-format-get-openapi.md
- name: Sound Cloud Get Users Favorites. Format
  x-api-slug: sound-cloud
  description: Returns a collection of tracks favorited by the user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites.{format}
  tags: Users,Favorites,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavorites-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavorites-format-get-openapi.md
- name: Sound Cloud Put Users Favorites Track . Format
  x-api-slug: sound-cloud
  description: Adds the given track to the given user's list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites/{track_id}.{format}
  tags: Users,Favorites,Track,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-format-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-format-put-openapi.md
- name: Sound Cloud Delete Users Favorites Track . Format
  x-api-slug: sound-cloud
  description: Deletes the given track from the given user's list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/favorites/{track_id}.{format}
  tags: Users,Favorites,Track,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-format-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idfavoritestrack-id-format-delete-openapi.md
- name: Sound Cloud Get Users Groups. Format
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/groups.{format}
  tags: Users,Groups,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idgroups-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idgroups-format-get-openapi.md
- name: Sound Cloud Get Users Playlists. Format
  x-api-slug: sound-cloud
  description: Returns a collection of playlists created by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/playlists.{format}
  tags: Users,Playlists,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idplaylists-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/usersuser-idplaylists-format-get-openapi.md
- name: Sound Cloud Get Groups Users. Format
  x-api-slug: sound-cloud
  description: Returns a combined collection of moderators, members and contributors
    of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/users.{format}
  tags: Groups,Users,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/groupsgroup-idusers-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/groupsgroup-idusers-format-get-openapi.md
- name: Sound Cloud
  x-api-slug: sound-cloud
  description: SoundCloud is a music and podcast streaming platform that lets you
    listen to millions of songs from around the world, or upload your own. Start listening
    now!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com//
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/soundcloud/openapi.md
x-common:
- type: x-base
  url: https://api.soundcloud.com
- type: x-blog
  url: http://blog.soundcloud.com
- type: x-blog-rss
  url: http://blog.soundcloud.com/feed/
- type: x-console
  url: https://developers.soundcloud.com/console
- type: x-crunchbase
  url: https://crunchbase.com/organization/soundcloud
- type: x-crunchbase
  url: http://www.crunchbase.com/company/soundcloud
- type: x-developer
  url: http://developers.soundcloud.com
- type: x-github
  url: https://github.com/soundcloud
- type: x-linkedin
  url: https://www.linkedin.com/company/soundcloud/
- type: x-pricing
  url: https://on.soundcloud.com/
- type: x-privacy
  url: https://soundcloud.com/pages/privacy
- type: x-support
  url: https://soundcloud.com/imprint
- type: x-terms-of-service
  url: https://soundcloud.com/terms-of-use
- type: x-twitter
  url: https://twitter.com/soundcloudapi
- type: x-twitter
  url: https://twitter.com/SoundCloud
- type: x-website
  url: http://soundcloud.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---