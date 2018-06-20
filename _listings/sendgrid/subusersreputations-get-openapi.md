---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Subusers Reputations
  description: |-
    Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received. When a bounce, spam report, or other negative action happens on a sent email, it will effect your sender rating.

    This endpoint allows you to request the reputations for your subusers.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subusers:
    get:
      summary: Get Subusers
      description: |-
        This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

        For more information about Subusers:

        * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
        * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
      operationId: GET_subusers
      x-api-path-slug: subusers-get
      parameters:
      - in: query
        name: limit
        description: The number of results you would like to get in each request
      - in: query
        name: offset
        description: The number of subusers to skip
      - in: query
        name: username
        description: The username of this subuser
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
    post:
      summary: Add Subusers
      description: |-
        This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

        For more information about Subusers:

        * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
        * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
      operationId: POST_subusers
      x-api-path-slug: subusers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
  /subusers/reputations:
    get:
      summary: Get Subusers Reputations
      description: |-
        Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received. When a bounce, spam report, or other negative action happens on a sent email, it will effect your sender rating.

        This endpoint allows you to request the reputations for your subusers.
      operationId: subusers.reputations.get
      x-api-path-slug: subusersreputations-get
      parameters:
      - in: query
        name: usernames
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Reputations
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