---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Subusers
  description: |-
    This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
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