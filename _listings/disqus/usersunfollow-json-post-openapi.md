---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Users Unfollow
  description: Users Unfollow
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
  /users/listFollowingForums.json:
    get:
      summary: Users ListFollowingForums
      description: Users ListFollowingForums
      operationId: users-listfollowingforums
      x-api-path-slug: userslistfollowingforums-json-get
      parameters:
      - in: query
        name: attach
        description: 'Defaults to []                         Choices: followsForum,
          forumCanDisableAds, forumForumCategory, counters, forumDaysAlive, forumFeatures,
          forumIntegration, forumNewPolicy, forumPermissions'
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
      - Forums
  /users/listForums.json:
    get:
      summary: Users ListForums
      description: Users ListForums
      operationId: users-listforums
      x-api-path-slug: userslistforums-json-get
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
      - Forums
  /users/listModeratedChannels.json:
    get:
      summary: Users ListModeratedChannels
      description: Users ListModeratedChannels
      operationId: users-listmoderatedchannels
      x-api-path-slug: userslistmoderatedchannels-json-get
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
        name: excludeOwned
        description: Defaults to false                         Whether to exclude
          Channels that the user owns from the results
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
  /users/listMostActiveForums.json:
    get:
      summary: Users ListMostActiveForums
      description: Users ListMostActiveForums
      operationId: users-listmostactiveforums
      x-api-path-slug: userslistmostactiveforums-json-get
      parameters:
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
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
  /users/listOwnedChannels.json:
    get:
      summary: Users ListOwnedChannels
      description: Users ListOwnedChannels
      operationId: users-listownedchannels
      x-api-path-slug: userslistownedchannels-json-get
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
  /users/listPosts.json:
    get:
      summary: Users ListPosts
      description: Users ListPosts
      operationId: users-listposts
      x-api-path-slug: userslistposts-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: filters
        description: 'Defaults to []                         Valid values are: 1:
          Is_Anonymous 2: Has_Link 3: Has_Low_Rep_Author 4: Has_Bad_Word 5: Is_Flagged
          6: No_Issue 7: Is_Toxic'
        type: string
      - in: query
        name: include
        description: 'Defaults to [  approved]                         Choices: unapproved,
          approved, spam, deleted, flagged, highlighted'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to desc                         Choices: asc, desc'
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
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
  /users/removeFollower.json:
    post:
      summary: Users RemoveFollower
      description: Users RemoveFollower
      operationId: users-removefollower
      x-api-path-slug: usersremovefollower-json-post
      parameters:
      - in: query
        name: follower
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/report.json:
    post:
      summary: Users Report
      description: Users Report
      operationId: users-report
      x-api-path-slug: usersreport-json-post
      parameters:
      - in: query
        name: reason
        description: 'Valid values are: 0: HARASSMENT 1: SPAM 2: INAPPROPRIATE_CONTENT
          3: THREAT 4: IMPERSONATION 5: PRIVATE_INFORMATION 6: DISAGREE'
        type: string
      - in: query
        name: user
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Users
  /users/unfollow.json:
    post:
      summary: Users Unfollow
      description: Users Unfollow
      operationId: users-unfollow
      x-api-path-slug: usersunfollow-json-post
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