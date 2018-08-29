---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
  description: the-reddit-api-allows-you-to-access-the-user-submitted-and-rated-stories-on-reddit-com--it-also-provides-advanced-functionality-including-user-account-information-and-subreddit-moderation-
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/where:
    get&nbsp;:
      summary: Get Users Where
      description: Get all user subreddits.
      operationId: get&nbsp;UsersWhere
      x-api-path-slug: userswhere-getnbsp
      parameters:
      - in: query
        name: after
        description: fullname of a thing
        type: string
      - in: query
        name: before
        description: fullname of a thing
        type: string
      - in: query
        name: count
        description: 'a positive integer (default: 0)'
        type: string
      - in: query
        name: limit
        description: 'the maximum number of items desired (default: 25, maximum: 100)'
        type: string
      - in: query
        name: show
        description: (optional) the string all
        type: string
      - in: query
        name: sr_detail
        description: (optional) expand subreddits
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Where
---