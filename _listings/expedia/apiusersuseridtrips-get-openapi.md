---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia (Internal Only)
  description: (Internal Only) Returns array of trips for passed userId
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/users/{userId}/trips/{tripId}:
    get:
      summary: (Internal Only)
      description: (Internal Only) Retrieve trip (tripId) for given customer (userId)
      operationId: trips-user-trips
      x-api-path-slug: apiusersuseridtripstripid-get
      parameters:
      - in: query
        name: currencyCode
        description: currency paramater
      - in: query
        name: decimalPlaceCount
        description: Decimal place count for the expected amount
      - in: query
        name: decorator
        description: Nullifies complex elements of a Trip with exception of Price
          related elements and their parents
      - in: query
        name: email
        description: To pull a guest itinerary specify the email address associated
          with the trip
      - in: query
        name: expectedAmount
        description: Expected Amount during car cancellation
      - in: path
        name: tripId
        description: Trip ID
      - in: query
        name: useCache
        description: An optional flag to make a cached read trip call
      - in: path
        name: userId
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users
  /api/users/{userId}/trips:
    get:
      summary: (Internal Only)
      description: (Internal Only) Returns array of trips for passed userId
      operationId: trips-by-user-id
      x-api-path-slug: apiusersuseridtrips-get
      parameters:
      - in: path
        name: userId
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Travel
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