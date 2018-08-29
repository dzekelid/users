---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Users ListFollowingChannels
  description: Users ListFollowingChannels
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forums/listUsers.json:
    get:
      summary: Forums ListUsers
      description: Forums ListUsers
      operationId: forums-listusers
      x-api-path-slug: forumslistusers-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Forums
      - Lists
      - Users
  /users/details.json:
    get:
      summary: Users Details
      description: Users Details
      operationId: users-details
      x-api-path-slug: usersdetails-json-get
      parameters:
      - in: query
        name: attach
        description: 'Defaults to []                         Choices: userFlaggedUser'
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/follow.json:
    post:
      summary: Users Follow
      description: Users Follow
      operationId: users-follow
      x-api-path-slug: usersfollow-json-post
      parameters:
      - in: query
        name: target
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/listActiveForums.json:
    get:
      summary: Users ListActiveForums
      description: Users ListActiveForums
      operationId: users-listactiveforums
      x-api-path-slug: userslistactiveforums-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/listActivity.json:
    get:
      summary: Users ListActivity
      description: Users ListActivity
      operationId: users-listactivity
      x-api-path-slug: userslistactivity-json-get
      parameters:
      - in: query
        name: anon_user
        description: Defaults to null                         Looks up an anonymous
          user by unique hash
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: include
        description: 'Defaults to [  user,  replies,  following]                         Choices:
          user, replies, following'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to [  forum,  thread]                         You may
          specify relations to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/listFollowers.json:
    get:
      summary: Users ListFollowers
      description: Users ListFollowers
      operationId: users-listfollowers
      x-api-path-slug: userslistfollowers-json-get
      parameters:
      - in: query
        name: attach
        description: 'Defaults to []                         Choices: userFlaggedUser'
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/listFollowing.json:
    get:
      summary: Users ListFollowing
      description: Users ListFollowing
      operationId: users-listfollowing
      x-api-path-slug: userslistfollowing-json-get
      parameters:
      - in: query
        name: attach
        description: 'Defaults to []                         Choices: userFlaggedUser'
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/listFollowingChannels.json:
    get:
      summary: Users ListFollowingChannels
      description: Users ListFollowingChannels
      operationId: users-listfollowingchannels
      x-api-path-slug: userslistfollowingchannels-json-get
      parameters:
      - in: query
        name: attach
        description: 'Defaults to []                         Choices: followsForum,
          forumCanDisableAds, forumForumCategory, counters, forumDaysAlive, forumFeatures,
          forumIntegration, forumNewPolicy, forumPermissions, channel_categories'
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: excludeModerated
        description: Defaults to false                         Whether to exclude
          Channels that the user moderates fromthe results
        type: string
      - in: query
        name: excludeOwned
        description: Defaults to false                         Whether to exclude
          Channels that the user owns from the results
        type: string
      - in: query
        name: includeFollowedPrimaryForums
        description: Defaults to false                         Whether to include
          Channels where the user follows the primary forum
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
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