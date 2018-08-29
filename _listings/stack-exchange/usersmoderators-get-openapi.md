---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get User Moderators
  description: "Gets those users on a site who can exercise moderation powers.\n \nNote,
    employees of Stack Exchange Inc. will be returned if they have been granted moderation
    powers on a site even if they have never been appointed or elected explicitly.
    This method checks abilities, not the manner in which they were obtained.\n \nThe
    sorts accepted by this method operate on the follow fields of the user object:\n
    - reputation - reputation\n - creation - creation_date\n - name - display_name\n
    - modified - last_modified_date\n  reputation is the default sort.\n \n It is
    possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of users."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get Users
      description: "Returns all users on a site.\n \nThis method returns a list of
        users.\n \nThe sorts accepted by this method operate on the follow fields
        of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThe inname parameter lets consumers
        filter the results down to just those users with a certain substring in their
        display name. For example, inname=kevin will return all users with both users
        named simply \"Kevin\" or those with Kevin as one of (or part of) their names;
        such as \"Kevin Montrose\"."
      operationId: returns-all-users-on-a-site-this-method-returns-a-list-of-users-the-sorts-accepted-by-this-method-op
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/moderators:
    get:
      summary: Get User Moderators
      description: "Gets those users on a site who can exercise moderation powers.\n
        \nNote, employees of Stack Exchange Inc. will be returned if they have been
        granted moderation powers on a site even if they have never been appointed
        or elected explicitly. This method checks abilities, not the manner in which
        they were obtained.\n \nThe sorts accepted by this method operate on the follow
        fields of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThis method returns a list of users."
      operationId: gets-those-users-on-a-site-who-can-exercise-moderation-powers-note-employees-of-stack-exchange-inc-w
      x-api-path-slug: usersmoderators-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Moderators
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