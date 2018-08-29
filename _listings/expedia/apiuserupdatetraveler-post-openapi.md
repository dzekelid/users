---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Update
  description: Mobile API User Update Traveler
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
  /api/user/sign-in:
    post:
      summary: User Sign-In
      description: Mobile API User Sign-In
      operationId: signin-user
      x-api-path-slug: apiusersignin-post
      parameters:
      - in: formData
        name: email
        description: Email Address
      - in: formData
        name: firstTimeSigin
        description: Boolean to indicate if this is a first time sign-in
      - in: formData
        name: guestLoginWithItin
        description: When logging in with an Itin Number and Email set this field
          to True
      - in: formData
        name: includeFullPaymentProfile
      - in: formData
        name: itinNumber
        description: The Itinerary Number can be used instead of a password to authenticate
          the user
      - in: formData
        name: password
        description: User Password
      - in: formData
        name: profileOnly
        description: If true, dont provide username/password fields and just re-retrieve
          the currently signed on users profile
      - in: formData
        name: profileTypes
        description: This is a comma-separated list of profile types to retrieve when
          the login is processed
      - in: formData
        name: retrieveCoupons
        description: Whether to include user coupons in the response
      - in: formData
        name: staySignedIn
        description: Sign Me In checkbox
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users
  /api/user/profile:
    get:
      summary: Profile
      description: Mobile API User Profile
      operationId: profile-user
      x-api-path-slug: apiuserprofile-get
      parameters:
      - in: query
        name: profileTypes
        description: This is a comma-separated list of profile types to retrieve when
          the login is processed
      - in: query
        name: retrieveCoupons
        description: Whether to include user coupons in the response
      - in: query
        name: tuid
        description: The tuid of the user/account whose profile you would like
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users
  /api/user/create:
    post:
      summary: Create User
      description: Mobile API User Create
      operationId: create-user
      x-api-path-slug: apiusercreate-post
      parameters:
      - in: formData
        name: email
        description: Users email address
      - in: formData
        name: enrollInLoyalty
        description: Whether to enroll the user in loyalty
      - in: formData
        name: expediaEmailOptIn
        description: Whether to opt-in the users email to travel deals
      - in: formData
        name: firstName
        description: Users first name
      - in: formData
        name: lastName
        description: Users last name
      - in: formData
        name: middleName
        description: Users middle name
      - in: formData
        name: password
        description: Users password
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users
  /api/user/update-traveler:
    post:
      summary: Update
      description: Mobile API User Update Traveler
      operationId: update-traveler
      x-api-path-slug: apiuserupdatetraveler-post
      parameters:
      - in: formData
        name: birthDate
        description: TSA required field; passengers birth date
      - in: formData
        name: email
        description: This passengers email address
      - in: formData
        name: expediaEmailOptIn
        description: Whether to opt-in the users email to travel deals
      - in: formData
        name: firstName
        description: The first name of the traveler
      - in: formData
        name: gender
        description: TSA required field, MALE or FEMALE
      - in: formData
        name: knownTravelerNumber
        description: Passengers knownTravelerNumber(PreCheckNumber), a 9 digit number
      - in: formData
        name: lastName
        description: The last name of the traveler
      - in: formData
        name: middleName
        description: The middle name of the traveler
      - in: formData
        name: passengerCategory
        description: The passengers category
      - in: formData
        name: passportCountryCode
        description: Passport country, UPPERCASE three letter country code
      - in: formData
        name: password
        description: The password provided by the Expedia user
      - in: formData
        name: phone
        description: The phone number of the traveler
      - in: formData
        name: phoneCountryCode
        description: The country code of the phone number of the traveler
      - in: formData
        name: seatPreference
        description: Passengers seat preference
      - in: formData
        name: specialAssistanceOption
        description: Special assistance choice
      - in: formData
        name: title
        description: Title of passenger
      - in: formData
        name: TSARedressNumber
        description: Passengers TSA redress number, which is, in theory a 7 digit
          number
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