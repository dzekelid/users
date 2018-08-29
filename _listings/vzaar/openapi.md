---
swagger: "2.0"
x-collection-name: Vzaar
x-complete: 1
info:
  title: VZaar API
  description: vzaar-is-an-online-video-hosting-service-with-fantastic-features-that-are-designed-for-business--deliver-to-mobile-or-the-web-straight-from-your-site-
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/users/{username}.{format}:
    get:
      summary: Get Api Users Username
      description: nnThis API call returns the users public details along with its
        relevant metadata.nn
      operationId: getApiUsersUsername.Format
      x-api-path-slug: apiusersusername-format-get
      parameters:
      - in: query
        name: 'username is the vzaar login name for the user. Note: This must be the
          actual username and not the email address'
      responses:
        200:
          description: OK
      tags:
      - Api
      - Users
      - Username
      - Format
---