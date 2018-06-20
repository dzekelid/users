---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Post Users User Addresses
  description: Creates a new UserAddress.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/favorites/listings:
    get:
      summary: Get Users User Favorites Listings
      description: Finds all favorite listings for a user
      operationId: getUsersUserFavoritesListings
      x-api-path-slug: usersuser-idfavoriteslistings-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
  /users/{user_id}/favorites/listings/{listing_id}:
    get:
      summary: Get Users User Favorites Listings Listing
      description: Finds a favorite listing for a user
      operationId: getUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-get
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
    post:
      summary: Post Users User Favorites Listings Listing
      description: Creates a new favorite listing for a user
      operationId: postUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-post
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
    delete:
      summary: Delete Users User Favorites Listings Listing
      description: Delete a favorite listing for a user
      operationId: deleteUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-delete
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
  /users/{user_id}/favorites/users:
    get:
      summary: Get Users User Favorites Users
      description: Finds all favorite users for a user
      operationId: getUsersUserFavoritesUsers
      x-api-path-slug: usersuser-idfavoritesusers-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
  /users/{user_id}/favorites/users/{target_user_id}:
    get:
      summary: Get Users User Favorites Users Target User
      description: Finds a favorite user for a user
      operationId: getUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-get
      parameters:
      - in: path
        name: target_user_id
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
    post:
      summary: Post Users User Favorites Users Target User
      description: Creates a new favorite listing for a user
      operationId: postUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-post
      parameters:
      - in: path
        name: target_user_id
      - in: query
        name: target_user_id
      - in: path
        name: user_id
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
    delete:
      summary: Delete Users User Favorites Users Target User
      description: Delete a favorite listing for a user
      operationId: deleteUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-delete
      parameters:
      - in: path
        name: target_user_id
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
  /users/{user_id}/recommended_listings:
    get:
      summary: Get Users User Recommended Listings
      description: Get recommended listings for an authenticated member. The number
        of listings returned may not match the specified limit if there is no activity
        from recommended shops.
      operationId: getUsersUserRecommendedListings
      x-api-path-slug: usersuser-idrecommended-listings-get
      parameters:
      - in: query
        name: excluded_listing_ids
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
  /users/{user_id}/recommended_listings/rejects/{listing_ids}:
    post:
      summary: Post Users User Recommended Listings Rejects Listing S
      description: Registers rejections of recommended listings. Affects future recommended
        listings.
      operationId: postUsersUserRecommendedListingsRejectsListingS
      x-api-path-slug: usersuser-idrecommended-listingsrejectslisting-ids-post
      parameters:
      - in: path
        name: listing_ids
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
      - Rejects
      - Listings
  /users/{user_id}/recommended_listings/views/{listing_ids}:
    post:
      summary: Post Users User Recommended Listings Views Listing S
      description: Register viewings of recommended listings. Affects future recommended
        listings.
      operationId: postUsersUserRecommendedListingsViewsListingS
      x-api-path-slug: usersuser-idrecommended-listingsviewslisting-ids-post
      parameters:
      - in: path
        name: listing_ids
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
      - Views
      - Listings
  /users/{user_id}/treasuries:
    get:
      summary: Get Users User Treasuries
      description: Get a user's Treasuries
      operationId: getUsersUserTreasuries
      x-api-path-slug: usersuser-idtreasuries-get
      parameters:
      - in: query
        name: detail_level
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: maturity
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: sort_on
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: sort_order
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Treasuries
  /users/{user_id}:
    get:
      summary: Get Users User
      description: Retrieves a User by id.
      operationId: getUsersUser
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/shops:
    get:
      summary: Get Users User Shops
      description: Retrieves a set of Shop objects associated to a User.
      operationId: getUsersUserShops
      x-api-path-slug: usersuser-idshops-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Shops
  /users/{user_id}/favored-by:
    get:
      summary: Get Users User Favored By
      description: Retrieves a set of FavoriteUser objects associated to a User.
      operationId: getUsersUserFavoredBy
      x-api-path-slug: usersuser-idfavoredby-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favored-by
  /users/{user_id}/feedback/as-subject:
    get:
      summary: Get Users User Feedback As Subject
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsSubject
      x-api-path-slug: usersuser-idfeedbackassubject-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-subject
  /users/{user_id}/feedback/as-author:
    get:
      summary: Get Users User Feedback As Author
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsAuthor
      x-api-path-slug: usersuser-idfeedbackasauthor-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-author
  /users/{user_id}/feedback/as-buyer:
    get:
      summary: Get Users User Feedback As Buyer
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsBuyer
      x-api-path-slug: usersuser-idfeedbackasbuyer-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-buyer
  /users/{user_id}/feedback/as-seller:
    get:
      summary: Get Users User Feedback As Seller
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsSeller
      x-api-path-slug: usersuser-idfeedbackasseller-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-seller
  /users/{user_id}/orders:
    get:
      summary: Get Users User Orders
      description: Retrieves a set of Order objects associated to a User.
      operationId: getUsersUserOrders
      x-api-path-slug: usersuser-idorders-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders
  /users/{user_id}/receipts:
    get:
      summary: Get Users User Receipts
      description: Retrieves a set of Receipt objects associated to a User.
      operationId: getUsersUserReceipts
      x-api-path-slug: usersuser-idreceipts-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Receipts
  /users/{user_id}/transactions:
    get:
      summary: Get Users User Transactions
      description: Retrieves a set of Transaction objects associated to a User.
      operationId: getUsersUserTransactions
      x-api-path-slug: usersuser-idtransactions-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Transactions
  /users/{user_id}/charges:
    get:
      summary: Get Users User Charges
      description: Retrieves a set of BillCharge objects associated to a User.
      operationId: getUsersUserCharges
      x-api-path-slug: usersuser-idcharges-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Charges
  /users/{user_id}/payments:
    get:
      summary: Get Users User Payments
      description: Retrieves a set of BillPayment objects associated to a User.
      operationId: getUsersUserPayments
      x-api-path-slug: usersuser-idpayments-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
  /users/{user_id}/shipping/templates:
    get:
      summary: Get Users User Shipping Templates
      description: Retrieves a set of ShippingTemplate objects associated to a User.
      operationId: getUsersUserShippingTemplates
      x-api-path-slug: usersuser-idshippingtemplates-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Shipping
      - Templates
  /users/{user_id}/payments/templates:
    get:
      summary: Get Users User Payments Templates
      description: Retrieves a set of PaymentTemplate objects associated to a User.
      operationId: getUsersUserPaymentsTemplates
      x-api-path-slug: usersuser-idpaymentstemplates-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
      - Templates
  /users/{user_id}/addresses:
    get:
      summary: Get Users User Addresses
      description: Retrieves a set of UserAddress objects associated to a User.
      operationId: getUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
    post:
      summary: Post Users User Addresses
      description: Creates a new UserAddress.
      operationId: postUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-post
      parameters:
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: second_line
      - in: query
        name: state
      - in: path
        name: user_id
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
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