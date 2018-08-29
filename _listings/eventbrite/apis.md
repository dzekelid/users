---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite brings people together through live experiences. Discover
  events that match your passions, or create your own with online ticketing tools.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
x-kinRank: "9"
x-alexaRank: "643"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Get Users Me Notifications
  x-api-slug: eventbrite
  description: Gets a paginated response of notification objects for a determined
    user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/me/notifications/
  tags: Users,Me,Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersmenotifications-get-openapi.md
- name: Eventbrite Get Users User Organizations
  x-api-slug: eventbrite
  description: |-
    Returns a continuated list of organizations
    accessible to the current user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/organizations/
  tags: Users,:user,Organizations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-idorganizations-get-openapi.md
- name: Eventbrite Get Users User Tracking Beacons
  x-api-slug: eventbrite
  description: Returns the list of tracking_beacon for the user :user_id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/tracking_beacons/
  tags: Users,:user,Tracking,Beacons
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-idtracking-beacons-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-idtracking-beacons-get-openapi.md
- name: Eventbrite Get Users
  x-api-slug: eventbrite
  description: Returns a user for the specified user as user. If you want to get details
    about the currently authenticated user, use /users/me/.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersid-get-openapi.md
- name: Eventbrite Get Users Orders
  x-api-slug: eventbrite
  description: Returns a paginated response of orders, under the key orders, of all
    orders the user has placed (i.e. where the user was the person buying the tickets).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/orders/
  tags: Users,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidorders-get-openapi.md
- name: Eventbrite Get Users Organizers
  x-api-slug: eventbrite
  description: Returns a paginated response of organizer objects that are owned by
    the user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/organizers/
  tags: Users,Organizers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidorganizers-get-openapi.md
- name: Eventbrite Get Users Owned Events
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of events, under
    the key events, of all events the user owns (i.e. events they are organising)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/owned_events/
  tags: Users,Owned,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidowned-events-get-openapi.md
- name: Eventbrite Get Users Events
  x-api-slug: eventbrite
  description: Returns a paginated response of events, under the key events, of all
    events the user has access to
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/events/
  tags: Users,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidevents-get-openapi.md
- name: Eventbrite Get Users Venues
  x-api-slug: eventbrite
  description: Returns a paginated response of venue objects that are owned by the
    user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/venues/
  tags: Users,Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidvenues-get-openapi.md
- name: Eventbrite Get Users Owned Event Attendees
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of attendees,
    under the key attendees, of attendees visiting any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/owned_event_attendees/
  tags: Users,Owned,Event,Attendees
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidowned-event-attendees-get-openapi.md
- name: Eventbrite Get Users Owned Event Orders
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of orders,
    under the key orders, of orders placed against any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/owned_event_orders/
  tags: Users,Owned,Event,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidowned-event-orders-get-openapi.md
- name: Eventbrite Get Users Contact Lists
  x-api-slug: eventbrite
  description: |-
    Returns a list of contact_list that the user owns as the key
    contact_lists.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/
  tags: Users,Contact,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-lists-get-openapi.md
- name: Eventbrite Post Users Contact Lists
  x-api-slug: eventbrite
  description: |-
    Makes a new contact_list for the user and returns it as
    contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/
  tags: Users,Contact,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-lists-post-openapi.md
- name: Eventbrite Get Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: Gets a user&#8217;s contact_list by ID as contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-id-get-openapi.md
- name: Eventbrite Post Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: Updates the contact_list and returns it as contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-id-post-openapi.md
- name: Eventbrite Delete Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-id-delete-openapi.md
- name: Eventbrite Get Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: |-
    Returns the contacts on the contact list
    as contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-get-openapi.md
- name: Eventbrite Post Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: 'Adds a new contact to the contact list. Returns {&quot;created&quot;:
    true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-post-openapi.md
- name: Eventbrite Delete Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: |-
    Deletes the specified contact from the contact list.
    Returns {&quot;deleted&quot;: true}.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-delete-openapi.md
- name: Eventbrite Get Users Bookmarks
  x-api-slug: eventbrite
  description: Gets all the user&#8217;s saved events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/bookmarks/
  tags: Users,Bookmarks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidbookmarks-get-openapi.md
- name: Eventbrite Post Users Bookmarks Save
  x-api-slug: eventbrite
  description: 'Adds a new bookmark for the user. Returns {&quot;created&quot;: true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/bookmarks/save/
  tags: Users,Bookmarks,Save
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidbookmarkssave-post-openapi.md
- name: Eventbrite Post Users Bookmarks Unsave
  x-api-slug: eventbrite
  description: 'Removes the specified bookmark from the event for the user. Returns
    {&quot;deleted&quot;: true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/bookmarks/unsave/
  tags: Users,Bookmarks,Unsave
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidbookmarksunsave-post-openapi.md
- name: Eventbrite Get Users User Ticket Groups
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of ticket_group for the specified user.
    The alias me (/users/me/) may be used to refer to the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/ticket_groups/
  tags: Users,:user,Ticket,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-idticket-groups-get-openapi.md
- name: Eventbrite Post Users User Events Event Ticket Classes Ticket Class Ticket
    Groups
  x-api-slug: eventbrite
  description: |-
    Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
    belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
    If the list provided is empty, remove this ticket class from every ticket group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/
  tags: Users,:user,Events,:event,Ticket,Classes,:ticket,Class,Ticket,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-openapi.md
- name: Eventbrite Get Users User Discounts
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of cross_event_discount for the specified user.
    This operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/discounts/
  tags: Users,:user,Discounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-iddiscounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersuser-iddiscounts-get-openapi.md
- name: Eventbrite Get Users Assortment
  x-api-slug: eventbrite
  description: Retrieve the assortment for the user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/assortment/
  tags: Users,Assortment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidassortment-get-openapi.md
- name: Eventbrite Post Users Assortment
  x-api-slug: eventbrite
  description: |-
    Set a user&#8217;s assortment and returns the assortment for the specified
    user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/assortment/
  tags: Users,Assortment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/usersidassortment-post-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite brings people together through live experiences. Discover
    events that match your passions, or create your own with online ticketing tools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-crunchbase
  url: https://crunchbase.com/organization/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-twitter
  url: https://twitter.com/eventbrite
- type: x-website
  url: http://eventbriteapi.com
- type: x-website
  url: http://developer.eventbrite.com/
- type: x-website
  url: http://eventbrite.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---