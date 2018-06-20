---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 1
info:
  title: CloudFlare
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user:
    get:
      summary: User details
      description: User detailsn
      operationId: cloudflare-user-api
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Update part of your user details
      description: Update part of your user details
      operationId: cloudflare-user-api
      x-api-path-slug: user-patch
      parameters:
      - in: query
        name: country
        description: The country in which the user lives
      - in: query
        name: first_name
        description: Users first nameJohn
      - in: query
        name: last_name
        description: Users last nameAppleseed
      - in: query
        name: telephone
        description: Users telephone number+1 123-123-1234
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      - in: query
        name: zipcode
        description: The zipcode or postal code where the user lives
      responses:
        200:
          description: OK
      tags:
      - Users
---