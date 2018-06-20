---
name: Etsy
x-slug: etsy
description: Find handmade, vintage, and unique goods that express who you are.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
x-kinRank: "9"
x-alexaRank: "187"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/apis.md
specificationVersion: "0.14"
apis:
- name: Etsy Get Users User Favorites Listings
  x-api-slug: etsy
  description: Finds all favorite listings for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoriteslistings-get-openapi.md
- name: Etsy Get Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Finds a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-get-openapi.md
- name: Etsy Post Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Creates a new favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-post-openapi.md
- name: Etsy Delete Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Delete a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-delete-openapi.md
- name: Etsy Get Users User Favorites Users
  x-api-slug: etsy
  description: Finds all favorite users for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/users
  tags: Users,Favorites,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoritesusers-get-openapi.md
- name: Etsy Get Users User Favorites Users Target User
  x-api-slug: etsy
  description: Finds a favorite user for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-get-openapi.md
- name: Etsy Post Users User Favorites Users Target User
  x-api-slug: etsy
  description: Creates a new favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-post-openapi.md
- name: Etsy Delete Users User Favorites Users Target User
  x-api-slug: etsy
  description: Delete a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-delete-openapi.md
- name: Etsy Get Users User Recommended Listings
  x-api-slug: etsy
  description: Get recommended listings for an authenticated member. The number of
    listings returned may not match the specified limit if there is no activity from
    recommended shops.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings
  tags: Users,Recommended,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idrecommended-listings-get-openapi.md
- name: Etsy Post Users User Recommended Listings Rejects Listing S
  x-api-slug: etsy
  description: Registers rejections of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings/rejects/{listing_ids}
  tags: Users,Recommended,Listings,Rejects,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idrecommended-listingsrejectslisting-ids-post-openapi.md
- name: Etsy Post Users User Recommended Listings Views Listing S
  x-api-slug: etsy
  description: Register viewings of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings/views/{listing_ids}
  tags: Users,Recommended,Listings,Views,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idrecommended-listingsviewslisting-ids-post-openapi.md
- name: Etsy Get Users User Treasuries
  x-api-slug: etsy
  description: Get a user's Treasuries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/treasuries
  tags: Users,Treasuries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idtreasuries-get-openapi.md
- name: Etsy Get Users User
  x-api-slug: etsy
  description: Retrieves a User by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-id-get-openapi.md
- name: Etsy Get Users User Shops
  x-api-slug: etsy
  description: Retrieves a set of Shop objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/shops
  tags: Users,Shops
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idshops-get-openapi.md
- name: Etsy Get Users User Favored By
  x-api-slug: etsy
  description: Retrieves a set of FavoriteUser objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favored-by
  tags: Users,Favored-by
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfavoredby-get-openapi.md
- name: Etsy Get Users User Feedback As Subject
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/feedback/as-subject
  tags: Users,Feedback,As-subject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfeedbackassubject-get-openapi.md
- name: Etsy Get Users User Feedback As Author
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/feedback/as-author
  tags: Users,Feedback,As-author
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfeedbackasauthor-get-openapi.md
- name: Etsy Get Users User Feedback As Buyer
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/feedback/as-buyer
  tags: Users,Feedback,As-buyer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfeedbackasbuyer-get-openapi.md
- name: Etsy Get Users User Feedback As Seller
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/feedback/as-seller
  tags: Users,Feedback,As-seller
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idfeedbackasseller-get-openapi.md
- name: Etsy Get Users User Orders
  x-api-slug: etsy
  description: Retrieves a set of Order objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/orders
  tags: Users,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idorders-get-openapi.md
- name: Etsy Get Users User Receipts
  x-api-slug: etsy
  description: Retrieves a set of Receipt objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/receipts
  tags: Users,Receipts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idreceipts-get-openapi.md
- name: Etsy Get Users User Transactions
  x-api-slug: etsy
  description: Retrieves a set of Transaction objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/transactions
  tags: Users,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idtransactions-get-openapi.md
- name: Etsy Get Users User Charges
  x-api-slug: etsy
  description: Retrieves a set of BillCharge objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/charges
  tags: Users,Charges
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idcharges-get-openapi.md
- name: Etsy Get Users User Payments
  x-api-slug: etsy
  description: Retrieves a set of BillPayment objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/payments
  tags: Users,Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idpayments-get-openapi.md
- name: Etsy Get Users User Shipping Templates
  x-api-slug: etsy
  description: Retrieves a set of ShippingTemplate objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/shipping/templates
  tags: Users,Shipping,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idshippingtemplates-get-openapi.md
- name: Etsy Get Users User Payments Templates
  x-api-slug: etsy
  description: Retrieves a set of PaymentTemplate objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/payments/templates
  tags: Users,Payments,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idpaymentstemplates-get-openapi.md
- name: Etsy Get Users User Addresses
  x-api-slug: etsy
  description: Retrieves a set of UserAddress objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/addresses
  tags: Users,Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idaddresses-get-openapi.md
- name: Etsy Post Users User Addresses
  x-api-slug: etsy
  description: Creates a new UserAddress.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/addresses
  tags: Users,Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idaddresses-post-openapi.md
- name: Etsy Post Users User Avatar
  x-api-slug: etsy
  description: Upload a new user avatar image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/avatar
  tags: Users,Avatar
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idavatar-post-openapi.md
- name: Etsy Get Users User Avatar Src
  x-api-slug: etsy
  description: Get avatar image source
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/avatar/src
  tags: Users,Avatar,Src
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idavatarsrc-get-openapi.md
- name: Etsy Get Users User Addresses User Address
  x-api-slug: etsy
  description: Retrieves a UserAddress by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idaddressesuser-address-id-get-openapi.md
- name: Etsy Put Users User Addresses User Address
  x-api-slug: etsy
  description: Updates a UserAddress with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idaddressesuser-address-id-put-openapi.md
- name: Etsy Delete Users User Addresses User Address
  x-api-slug: etsy
  description: Deletes the UserAddress with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/usersuser-idaddressesuser-address-id-delete-openapi.md
- name: Etsy Get Featured Users
  x-api-slug: etsy
  description: Finds all FeaturedUser.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///featured/users
  tags: Featured,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/featuredusers-get-openapi.md
- name: Etsy Get Featured Users Featured User
  x-api-slug: etsy
  description: Retrieves a FeaturedUser by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///featured/users/{featured_user_id}
  tags: Featured,Users,Featured,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/featuredusersfeatured-user-id-get-openapi.md
- name: Etsy
  x-api-slug: etsy
  description: Etsy is a handmade marketplace. The Etsy API lets developers tap into
    the Etsy community, building their own Etsy-powered applications for the web,
    desktop and mobile devices. Applications built on the API will connect buyers
    with sellers, promote the handmade lifestyle, and support the craftspeople who
    sell on Etsy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/etsy/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/etsy.json
- type: x-application-gallery
  url: https://www.etsy.com/apps/
- type: x-base
  url: https://openapi.etsy.com/
- type: x-blog
  url: http://www.etsy.com/blog/en/
- type: x-blog-rss
  url: https://blog.etsy.com/en/feed/
- type: x-copyright
  url: https://www.etsy.com/help/article/482/?ref=ftr
- type: x-crunchbase
  url: https://crunchbase.com/organization/etsy
- type: x-crunchbase
  url: http://www.crunchbase.com/company/etsy
- type: x-developer
  url: https://www.etsy.com/developers/
- type: x-email
  url: enaffiliates@etsy.com
- type: x-email
  url: selleraffiliate@etsy.com
- type: x-email
  url: developer@etsy.com
- type: x-email
  url: legal@etsy.com
- type: x-email
  url: dpo@etsy.com
- type: x-email
  url: dispute-resolution@etsy.com
- type: x-forum
  url: https://www.etsy.com/developers/discussion
- type: x-github
  url: https://github.com/etsy
- type: x-privacy
  url: https://www.etsy.com/help/article/480/?ref=ftr
- type: x-terms-of-service
  url: https://www.etsy.com/help/article/479/?ref=ftr
- type: x-transparency-report
  url: http://blog.etsy.com/news/files/2015/07/Etsy_TransparencyReport_2014.pdf
- type: x-twitter
  url: https://twitter.com/Etsy
- type: x-website
  url: http://www.etsy.com/
- type: x-website
  url: http://etsy.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---