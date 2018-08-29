---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Delete Users Contact Lists Contact List Contacts
  description: |-
    Deletes the specified contact from the contact list.
    Returns {&quot;deleted&quot;: true}.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/me/notifications/:
    get:
      summary: Get Users Me Notifications
      description: Gets a paginated response of notification objects for a determined
        user.
      operationId: getUsersMeNotifications
      x-api-path-slug: usersmenotifications-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me
      - Notifications
  /users/:user_id/organizations/:
    get:
      summary: Get Users User Organizations
      description: |-
        Returns a continuated list of organizations
        accessible to the current user.
      operationId: getUsersUserOrganizations
      x-api-path-slug: usersuser-idorganizations-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Organizations
  /users/:user_id/tracking_beacons/:
    get:
      summary: Get Users User Tracking Beacons
      description: Returns the list of tracking_beacon for the user :user_id
      operationId: getUsersUserTrackingBeacons
      x-api-path-slug: usersuser-idtracking-beacons-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Tracking
      - Beacons
  /users/{id}/:
    get:
      summary: Get Users
      description: Returns a user for the specified user as user. If you want to get
        details about the currently authenticated user, use /users/me/.
      operationId: getUsers
      x-api-path-slug: usersid-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{id}/orders/:
    get:
      summary: Get Users Orders
      description: Returns a paginated response of orders, under the key orders, of
        all orders the user has placed (i.e. where the user was the person buying
        the tickets).
      operationId: getUsersOrders
      x-api-path-slug: usersidorders-get
      parameters:
      - in: query
        name: '&#160;'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders
  /users/{id}/organizers/:
    get:
      summary: Get Users Organizers
      description: Returns a paginated response of organizer objects that are owned
        by the user.
      operationId: getUsersOrganizers
      x-api-path-slug: usersidorganizers-get
      parameters:
      - in: query
        name: hide_unsaved
        description: 'True: Will hide organizers flagged as &#8220;unsaved&#8221;False:
          Will show organizers regardless of unsaved flag (Default value)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Organizers
  /users/{id}/owned_events/:
    get:
      summary: Get Users Owned Events
      description: |-
        Returns a paginated response of events, under
        the key events, of all events the user owns (i.e. events they are organising)
      operationId: getUsersOwnedEvents
      x-api-path-slug: usersidowned-events-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Events
  /users/{id}/events/:
    get:
      summary: Get Users Events
      description: Returns a paginated response of events, under the key events, of
        all events the user has access to
      operationId: getUsersEvents
      x-api-path-slug: usersidevents-get
      parameters:
      - in: query
        name: currency_filter
        description: Filter event results by currency
        type: query
      - in: query
        name: event_group_id
        description: Filter event results by event_group_id
        type: query
      - in: query
        name: name_filter
        description: Filter event results by name
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: page_size
        description: Number of records in each page
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
          / orders
        type: query
      - in: query
        name: venue_filter
        description: Filter event results by venue IDs
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Events
  /users/{id}/venues/:
    get:
      summary: Get Users Venues
      description: Returns a paginated response of venue objects that are owned by
        the user.
      operationId: getUsersVenues
      x-api-path-slug: usersidvenues-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Venues
  /users/{id}/owned_event_attendees/:
    get:
      summary: Get Users Owned Event Attendees
      description: |-
        Returns a paginated response of attendees,
        under the key attendees, of attendees visiting any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventAttendees
      x-api-path-slug: usersidowned-event-attendees-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: status
        description: Limits results to either confirmed attendees or cancelled/refunded/etc
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Attendees
  /users/{id}/owned_event_orders/:
    get:
      summary: Get Users Owned Event Orders
      description: |-
        Returns a paginated response of orders,
        under the key orders, of orders placed against any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventOrders
      x-api-path-slug: usersidowned-event-orders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), or all
          (both) orders (Valid choices are: active, inactive, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Orders
  /users/{id}/contact_lists/:
    get:
      summary: Get Users Contact Lists
      description: |-
        Returns a list of contact_list that the user owns as the key
        contact_lists.
      operationId: getUsersContactLists
      x-api-path-slug: usersidcontact-lists-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
    post:
      summary: Post Users Contact Lists
      description: |-
        Makes a new contact_list for the user and returns it as
        contact_list.
      operationId: postUsersContactLists
      x-api-path-slug: usersidcontact-lists-post
      parameters:
      - in: query
        name: contact_list.name
        description: Name of the new contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
  /users/{id}/contact_lists/:contact_list_id/:
    get:
      summary: Get Users Contact Lists Contact List
      description: Gets a user&#8217;s contact_list by ID as contact_list.
      operationId: getUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    post:
      summary: Post Users Contact Lists Contact List
      description: Updates the contact_list and returns it as contact_list.
      operationId: postUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-post
      parameters:
      - in: query
        name: contact_list.name
        description: New name of the contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    delete:
      summary: Delete Users Contact Lists Contact List
      description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
      operationId: deleteUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
  /users/{id}/contact_lists/:contact_list_id/contacts/:
    get:
      summary: Get Users Contact Lists Contact List Contacts
      description: |-
        Returns the contacts on the contact list
        as contacts.
      operationId: getUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
    post:
      summary: Post Users Contact Lists Contact List Contacts
      description: 'Adds a new contact to the contact list. Returns {&quot;created&quot;:
        true}.'
      operationId: postUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-post
      parameters:
      - in: query
        name: contact.email
        description: Contact&#8217;s email address
        type: query
      - in: query
        name: contact.first_name
        description: Contact&#8217;s first name (or full name)
        type: query
      - in: query
        name: contact.last_name
        description: Contact&#8217;s last name
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
    delete:
      summary: Delete Users Contact Lists Contact List Contacts
      description: |-
        Deletes the specified contact from the contact list.
        Returns {&quot;deleted&quot;: true}.
      operationId: deleteUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-delete
      parameters:
      - in: query
        name: email
        description: Email address to remove
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
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