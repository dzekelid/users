---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Users Followers Contact . Format
  description: Checks if the user with contact_id is a follower of the given user.
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users.json:
    get:
      summary: Get Users
      description: Returns a collection of users
      operationId: getUsers.json
      x-api-path-slug: users-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}.json:
    get:
      summary: Get Users
      description: Returns a user by user id
      operationId: getUsersUser.json
      x-api-path-slug: usersuser-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/tracks.json:
    get:
      summary: Get Users Tracks
      description: Returns a collection of tracks uploaded by user id
      operationId: getUsersUserTracks.json
      x-api-path-slug: usersuser-idtracks-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tracks
  /users/{user_id}/comments.json:
    get:
      summary: Get Users Comments
      description: Returns a collection of comments made by user id
      operationId: getUsersUserComments.json
      x-api-path-slug: usersuser-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{user_id}/followings.json:
    get:
      summary: Get Users Followings
      description: Returns a collection of users the user with user id is following
      operationId: getUsersUserFollowings.json
      x-api-path-slug: usersuser-idfollowings-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
  /users/{user_id}/followings/{contact_id}.json:
    get:
      summary: Get Users Followings Contact
      description: Checks if the user with the id contact_id is in the givens user's
        list of contacts.
      operationId: getUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
    put:
      summary: Put Users Followings Contact
      description: Adds the user with the id contact_id to the givens user's list
        of contacts.
      operationId: putUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
    delete:
      summary: Delete Users Followings Contact
      description: Removes the user with the id contact_id from the givens user's
        list of contacts.
      operationId: deleteUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
  /users/{user_id}/followers.json:
    get:
      summary: Get Users Followers
      description: Returns a collection of users who follow the user with user id
      operationId: getUsersUserFollowers.json
      x-api-path-slug: usersuser-idfollowers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
  /users/{user_id}/followers/{contact_id}.json:
    get:
      summary: Get Users Followers Contact
      description: Checks if the user with contact_id is a follower of the given user.
      operationId: getUsersUserFollowersContact.json
      x-api-path-slug: usersuser-idfollowerscontact-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - Contact
  /users/{user_id}/favorites.json:
    get:
      summary: Get Users Favorites
      description: Returns a collection of tracks favorited by the user with user
        id
      operationId: getUsersUserFavorites.json
      x-api-path-slug: usersuser-idfavorites-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
  /users/{user_id}/favorites/{track_id}.json:
    put:
      summary: Put Users Favorites Track
      description: Adds the given track to the given user's list of favorites.
      operationId: putUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
    delete:
      summary: Delete Users Favorites Track
      description: Deletes the given track from the given user's list of favorites.
      operationId: deleteUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
  /users/{user_id}/groups.json:
    get:
      summary: Get Users Groups
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.json
      x-api-path-slug: usersuser-idgroups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /users/{user_id}/playlists.json:
    get:
      summary: Get Users Playlists
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.json
      x-api-path-slug: usersuser-idplaylists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
  /groups/{group_id}/users.json:
    get:
      summary: Get Groups Users
      description: Returns a combined collection of moderators, members and contributors
        of the group with group id
      operationId: getGroupsGroupUsers.json
      x-api-path-slug: groupsgroup-idusers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Users
  /users.{format}:
    get:
      summary: Get Users. Format
      description: Returns a collection of users
      operationId: getUsers.Format
      x-api-path-slug: users-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: q
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Format
  /users/{user_id}.{format}:
    get:
      summary: Get Users . Format
      description: Returns a user by user id
      operationId: getUsersUser.Format
      x-api-path-slug: usersuser-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - ""
      - Format
  /users/{user_id}/tracks.{format}:
    get:
      summary: Get Users Tracks. Format
      description: Returns a collection of tracks uploaded by user id
      operationId: getUsersUserTracks.Format
      x-api-path-slug: usersuser-idtracks-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tracks
      - ""
      - Format
  /users/{user_id}/comments.{format}:
    get:
      summary: Get Users Comments. Format
      description: Returns a collection of comments made by user id
      operationId: getUsersUserComments.Format
      x-api-path-slug: usersuser-idcomments-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
      - ""
      - Format
  /users/{user_id}/followings.{format}:
    get:
      summary: Get Users Followings. Format
      description: Returns a collection of users the user with user id is following
      operationId: getUsersUserFollowings.Format
      x-api-path-slug: usersuser-idfollowings-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - ""
      - Format
  /users/{user_id}/followings/{contact_id}.{format}:
    get:
      summary: Get Users Followings Contact . Format
      description: Checks if the user with the id contact_id is in the givens user's
        list of contacts.
      operationId: getUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
    put:
      summary: Put Users Followings Contact . Format
      description: Adds the user with the id contact_id to the givens user's list
        of contacts.
      operationId: putUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-put
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
    delete:
      summary: Delete Users Followings Contact . Format
      description: Removes the user with the id contact_id from the givens user's
        list of contacts.
      operationId: deleteUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-delete
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
  /users/{user_id}/followers.{format}:
    get:
      summary: Get Users Followers. Format
      description: Returns a collection of users who follow the user with user id
      operationId: getUsersUserFollowers.Format
      x-api-path-slug: usersuser-idfollowers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - ""
      - Format
  /users/{user_id}/followers/{contact_id}.{format}:
    get:
      summary: Get Users Followers Contact . Format
      description: Checks if the user with contact_id is a follower of the given user.
      operationId: getUsersUserFollowersContact.Format
      x-api-path-slug: usersuser-idfollowerscontact-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - Contact
      - ""
      - ""
      - Format
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---