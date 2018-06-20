---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Appointment Groups API List user participants
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List user participants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}/users
  tags: Appointment,Groups,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/appointment-groupsidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/appointment-groupsidusers-get-openapi.md
- name: Instructure Canvas Appointment Groups API
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/openapi.md
- name: Instructure Canvas Audit API Query by user.
  x-api-slug: instructure-canvas-audit-api
  description: Query by user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/authentication/users/{user_id}
  tags: Audit,Authentication,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/auditauthenticationusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/auditauthenticationusersuser-id-get-openapi.md
- name: Instructure Canvas Audit API
  x-api-slug: instructure-canvas-audit-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level participation data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level participation data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/activity
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idactivity-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level assignment data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level assignment data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/assignments
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level messaging data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level messaging data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/communication
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Communication
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idcommunication-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idcommunication-get-openapi.md
- name: Instructure Canvas Courses API Send a message to unsubmitted or submitted
    users for the quiz
  x-api-slug: instructure-canvas-courses-api
  description: Send a message to unsubmitted or submitted users for the quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id/submission_users/message
  tags: Courses,Course,Id,Quizzes,Id,Submission,Users,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idquizzesidsubmission-usersmessage-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idquizzesidsubmission-usersmessage-post-openapi.md
- name: Instructure Canvas Courses API List users in course
  x-api-slug: instructure-canvas-courses-api
  description: List users in course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/search_users
  tags: Courses,Course,Id,Search,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idsearch-users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idsearch-users-get-openapi.md
- name: Instructure Canvas Courses API List users in course
  x-api-slug: instructure-canvas-courses-api
  description: List users in course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/users
  tags: Courses,Course,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idusers-get-openapi.md
- name: Instructure Canvas Courses API Get single user
  x-api-slug: instructure-canvas-courses-api
  description: Get single user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/users/id
  tags: Courses,Course,Id,Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idusersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/coursescourse-idusersid-get-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/openapi.md
- name: Instructure Canvas Groups API List groups users
  x-api-slug: instructure-canvas-groups-api
  description: List groups users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users
  tags: Groups,Group,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusers-get-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/groupsgroup-idusersuser-id-put-openapi.md
- name: Instructure Canvas Groups API List users in group category
  x-api-slug: instructure-canvas-groups-api
  description: List users in group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/users
  tags: Group,Categories,Group,Category,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/group-categoriesgroup-category-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/group-categoriesgroup-category-idusers-get-openapi.md
- name: Instructure Canvas Groups API
  x-api-slug: instructure-canvas-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/openapi.md
- name: Instructure Canvas Users API List the activity stream
  x-api-slug: instructure-canvas-users-api
  description: List the activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/activity_stream
  tags: Users,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersactivity-stream-get-openapi.md
- name: Instructure Canvas Users API Hide all stream items
  x-api-slug: instructure-canvas-users-api
  description: Hide all stream items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream
  tags: Users,Self,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-stream-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-stream-delete-openapi.md
- name: Instructure Canvas Users API List the activity stream
  x-api-slug: instructure-canvas-users-api
  description: List the activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream
  tags: Users,Self,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-stream-get-openapi.md
- name: Instructure Canvas Users API Activity stream summary
  x-api-slug: instructure-canvas-users-api
  description: Activity stream summary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream/summary
  tags: Users,Self,Activity,Stream,Summary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-streamsummary-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-streamsummary-get-openapi.md
- name: Instructure Canvas Users API Hide a stream item
  x-api-slug: instructure-canvas-users-api
  description: Hide a stream item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream/{id}
  tags: Users,Self,Activity,Stream,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-streamid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfactivity-streamid-delete-openapi.md
- name: Instructure Canvas Users API List bookmarks
  x-api-slug: instructure-canvas-users-api
  description: List bookmarks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks
  tags: Users,Self,Bookmarks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarks-get-openapi.md
- name: Instructure Canvas Users API Create bookmark
  x-api-slug: instructure-canvas-users-api
  description: Create bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks
  tags: Users,Self,Bookmarks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarks-post-openapi.md
- name: Instructure Canvas Users API Delete bookmark
  x-api-slug: instructure-canvas-users-api
  description: Delete bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-delete-openapi.md
- name: Instructure Canvas Users API Get bookmark
  x-api-slug: instructure-canvas-users-api
  description: Get bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-get-openapi.md
- name: Instructure Canvas Users API Update bookmark
  x-api-slug: instructure-canvas-users-api
  description: Update bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfbookmarksid-put-openapi.md
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences/notification
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API Update preferences by category
  x-api-slug: instructure-canvas-users-api
  description: Update preferences by category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preference,Categories,Category
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put-openapi.md
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences/{notification}
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API Clear course nicknames
  x-api-slug: instructure-canvas-users-api
  description: Clear course nicknames.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames
  tags: Users,Self,Course,Nicknames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknames-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknames-delete-openapi.md
- name: Instructure Canvas Users API List course nicknames
  x-api-slug: instructure-canvas-users-api
  description: List course nicknames.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames
  tags: Users,Self,Course,Nicknames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknames-get-openapi.md
- name: Instructure Canvas Users API Remove course nickname
  x-api-slug: instructure-canvas-users-api
  description: Remove course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-delete-openapi.md
- name: Instructure Canvas Users API Get course nickname
  x-api-slug: instructure-canvas-users-api
  description: Get course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-get-openapi.md
- name: Instructure Canvas Users API Set course nickname
  x-api-slug: instructure-canvas-users-api
  description: Set course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfcourse-nicknamescourse-id-put-openapi.md
- name: Instructure Canvas Users API Reset course favorites
  x-api-slug: instructure-canvas-users-api
  description: Reset course favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses
  tags: Users,Self,Favorites,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescourses-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescourses-delete-openapi.md
- name: Instructure Canvas Users API List favorite courses
  x-api-slug: instructure-canvas-users-api
  description: List favorite courses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses
  tags: Users,Self,Favorites,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescourses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescourses-get-openapi.md
- name: Instructure Canvas Users API Remove course from favorites
  x-api-slug: instructure-canvas-users-api
  description: Remove course from favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses/{id}
  tags: Users,Self,Favorites,Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescoursesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescoursesid-delete-openapi.md
- name: Instructure Canvas Users API Add course to favorites
  x-api-slug: instructure-canvas-users-api
  description: Add course to favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses/{id}
  tags: Users,Self,Favorites,Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescoursesid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritescoursesid-post-openapi.md
- name: Instructure Canvas Users API Reset group favorites
  x-api-slug: instructure-canvas-users-api
  description: Reset group favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroups-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroups-delete-openapi.md
- name: Instructure Canvas Users API List favorite groups
  x-api-slug: instructure-canvas-users-api
  description: List favorite groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroups-get-openapi.md
- name: Instructure Canvas Users API Remove group from favorites
  x-api-slug: instructure-canvas-users-api
  description: Remove group from favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroupsid-delete-openapi.md
- name: Instructure Canvas Users API Add group to favorites
  x-api-slug: instructure-canvas-users-api
  description: Add group to favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroupsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselffavoritesgroupsid-post-openapi.md
- name: Instructure Canvas Users API List your groups
  x-api-slug: instructure-canvas-users-api
  description: List your groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/groups
  tags: Users,Self,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfgroups-get-openapi.md
- name: Instructure Canvas Users API List the TODO items
  x-api-slug: instructure-canvas-users-api
  description: List the todo items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/todo
  tags: Users,Self,Todo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselftodo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselftodo-get-openapi.md
- name: Instructure Canvas Users API List upcoming assignments, calendar events
  x-api-slug: instructure-canvas-users-api
  description: List upcoming assignments, calendar events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/upcoming_events
  tags: Users,Self,Upcoming,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfupcoming-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersselfupcoming-events-get-openapi.md
- name: Instructure Canvas Users API Show user details
  x-api-slug: instructure-canvas-users-api
  description: Show user details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}
  tags: Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersid-get-openapi.md
- name: Instructure Canvas Users API Edit a user
  x-api-slug: instructure-canvas-users-api
  description: Edit a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}
  tags: Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersid-put-openapi.md
- name: Instructure Canvas Users API Get custom colors
  x-api-slug: instructure-canvas-users-api
  description: Get custom colors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors
  tags: Users,Id,Colors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolors-get-openapi.md
- name: Instructure Canvas Users API Get custom color
  x-api-slug: instructure-canvas-users-api
  description: Get custom color.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors/asset_string
  tags: Users,Id,Colors,Asset,String
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolorsasset-string-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolorsasset-string-get-openapi.md
- name: Instructure Canvas Users API Update custom color
  x-api-slug: instructure-canvas-users-api
  description: Update custom color.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors/asset_string
  tags: Users,Id,Colors,Asset,String
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolorsasset-string-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidcolorsasset-string-put-openapi.md
- name: Instructure Canvas Users API Merge user into another user
  x-api-slug: instructure-canvas-users-api
  description: Merge user into another user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/merge_into/accounts/destination_account_id/users/{destination_user_id}
  tags: Users,Id,Merge,Into,Accounts,Destination,Account,Id,Users,Destination,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put-openapi.md
- name: Instructure Canvas Users API Merge user into another user
  x-api-slug: instructure-canvas-users-api
  description: Merge user into another user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/merge_into/destination_user_id
  tags: Users,Id,Merge,Into,Destination,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidmerge-intodestination-user-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidmerge-intodestination-user-id-put-openapi.md
- name: Instructure Canvas Users API Update user settings.
  x-api-slug: instructure-canvas-users-api
  description: Update user settings..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/settings
  tags: Users,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidsettings-get-openapi.md
- name: Instructure Canvas Users API Update user settings.
  x-api-slug: instructure-canvas-users-api
  description: Update user settings..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/settings
  tags: Users,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidsettings-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersidsettings-put-openapi.md
- name: Instructure Canvas Users API List avatar options
  x-api-slug: instructure-canvas-users-api
  description: List avatar options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/avatars
  tags: Users,User,Id,Avatars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idavatars-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idavatars-get-openapi.md
- name: Instructure Canvas Users API List calendar events for a user
  x-api-slug: instructure-canvas-users-api
  description: List calendar events for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/calendar_events
  tags: Users,User,Id,Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcalendar-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcalendar-events-get-openapi.md
- name: Instructure Canvas Users API List user communication channels
  x-api-slug: instructure-canvas-users-api
  description: List user communication channels.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels
  tags: Users,User,Id,Communication,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channels-get-openapi.md
- name: Instructure Canvas Users API Create a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Create a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels
  tags: Users,User,Id,Communication,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channels-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channels-post-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences/{notification}
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API List of preference categories
  x-api-slug: instructure-canvas-users-api
  description: List of preference categories.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preference_categories
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preference,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get-openapi.md
- name: Instructure Canvas Users API Delete a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Delete a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/id
  tags: Users,User,Id,Communication,Channels,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelsid-delete-openapi.md
- name: Instructure Canvas Users API Delete a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Delete a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}
  tags: Users,User,Id,Communication,Channels,Type,Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddress-delete-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences/notification
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API List content exports
  x-api-slug: instructure-canvas-users-api
  description: List content exports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports
  tags: Users,User,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exports-get-openapi.md
- name: Instructure Canvas Users API Export content
  x-api-slug: instructure-canvas-users-api
  description: Export content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports
  tags: Users,User,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exports-post-openapi.md
- name: Instructure Canvas Users API Show content export
  x-api-slug: instructure-canvas-users-api
  description: Show content export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports/id
  tags: Users,User,Id,Content,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-exportsid-get-openapi.md
- name: Instructure Canvas Users API List licenses
  x-api-slug: instructure-canvas-users-api
  description: List licenses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_licenses
  tags: Users,User,Id,Content,Licenses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-licenses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-licenses-get-openapi.md
- name: Instructure Canvas Users API List content migrations
  x-api-slug: instructure-canvas-users-api
  description: List content migrations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations
  tags: Users,User,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrations-get-openapi.md
- name: Instructure Canvas Users API Create a content migration
  x-api-slug: instructure-canvas-users-api
  description: Create a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations
  tags: Users,User,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrations-post-openapi.md
- name: Instructure Canvas Users API List migration issues
  x-api-slug: instructure-canvas-users-api
  description: List migration issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issues-get-openapi.md
- name: Instructure Canvas Users API Get a migration issue
  x-api-slug: instructure-canvas-users-api
  description: Get a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-get-openapi.md
- name: Instructure Canvas Users API Update a migration issue
  x-api-slug: instructure-canvas-users-api
  description: Update a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-put-openapi.md
- name: Instructure Canvas Users API Get a content migration
  x-api-slug: instructure-canvas-users-api
  description: Get a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/id
  tags: Users,User,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsid-get-openapi.md
- name: Instructure Canvas Users API Update a content migration
  x-api-slug: instructure-canvas-users-api
  description: Update a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/id
  tags: Users,User,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsid-put-openapi.md
- name: Instructure Canvas Users API List Migration Systems
  x-api-slug: instructure-canvas-users-api
  description: List migration systems.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/migrators
  tags: Users,User,Id,Content,Migrations,Migrators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsmigrators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcontent-migrationsmigrators-get-openapi.md
- name: Instructure Canvas Users API List courses for a user
  x-api-slug: instructure-canvas-users-api
  description: List courses for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/courses
  tags: Users,User,Id,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcourses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcourses-get-openapi.md
- name: Instructure Canvas Users API List assignments for user
  x-api-slug: instructure-canvas-users-api
  description: List assignments for user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/courses/course_id/assignments
  tags: Users,User,Id,Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Users API Delete custom data
  x-api-slug: instructure-canvas-users-api
  description: Delete custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-delete-openapi.md
- name: Instructure Canvas Users API Load custom data
  x-api-slug: instructure-canvas-users-api
  description: Load custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-get-openapi.md
- name: Instructure Canvas Users API Store custom data
  x-api-slug: instructure-canvas-users-api
  description: Store custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idcustom-datascope-put-openapi.md
- name: Instructure Canvas Users API List enrollments
  x-api-slug: instructure-canvas-users-api
  description: List enrollments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/enrollments
  tags: Users,User,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idenrollments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idenrollments-get-openapi.md
- name: Instructure Canvas Users API List features
  x-api-slug: instructure-canvas-users-api
  description: List features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features
  tags: Users,User,Id,Features
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeatures-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeatures-get-openapi.md
- name: Instructure Canvas Users API List enabled features
  x-api-slug: instructure-canvas-users-api
  description: List enabled features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/enabled
  tags: Users,User,Id,Features,Enabled
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesenabled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesenabled-get-openapi.md
- name: Instructure Canvas Users API Remove feature flag
  x-api-slug: instructure-canvas-users-api
  description: Remove feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-delete-openapi.md
- name: Instructure Canvas Users API Get feature flag
  x-api-slug: instructure-canvas-users-api
  description: Get feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-get-openapi.md
- name: Instructure Canvas Users API Set feature flag
  x-api-slug: instructure-canvas-users-api
  description: Set feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfeaturesflagsfeature-put-openapi.md
- name: Instructure Canvas Users API List files
  x-api-slug: instructure-canvas-users-api
  description: List files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files
  tags: Users,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfiles-get-openapi.md
- name: Instructure Canvas Users API Upload a file
  x-api-slug: instructure-canvas-users-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files
  tags: Users,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfiles-post-openapi.md
- name: Instructure Canvas Users API Get file
  x-api-slug: instructure-canvas-users-api
  description: Get file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files/id
  tags: Users,User,Id,Files,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfilesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfilesid-get-openapi.md
- name: Instructure Canvas Users API Get quota information
  x-api-slug: instructure-canvas-users-api
  description: Get quota information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files/quota
  tags: Users,User,Id,Files,Quota
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfilesquota-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfilesquota-get-openapi.md
- name: Instructure Canvas Users API List all folders
  x-api-slug: instructure-canvas-users-api
  description: List all folders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders
  tags: Users,User,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfolders-get-openapi.md
- name: Instructure Canvas Users API Create folder
  x-api-slug: instructure-canvas-users-api
  description: Create folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders
  tags: Users,User,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfolders-post-openapi.md
- name: Instructure Canvas Users API Resolve path
  x-api-slug: instructure-canvas-users-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/by_path
  tags: Users,User,Id,Folders,By,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersby-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersby-path-get-openapi.md
- name: Instructure Canvas Users API Resolve path
  x-api-slug: instructure-canvas-users-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/by_path/*full_path
  tags: Users,User,Id,Folders,By,Path,*full,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersby-pathfull-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersby-pathfull-path-get-openapi.md
- name: Instructure Canvas Users API Get folder
  x-api-slug: instructure-canvas-users-api
  description: Get folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/id
  tags: Users,User,Id,Folders,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idfoldersid-get-openapi.md
- name: Instructure Canvas Users API List user logins
  x-api-slug: instructure-canvas-users-api
  description: List user logins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/logins
  tags: Users,User,Id,Logins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idlogins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idlogins-get-openapi.md
- name: Instructure Canvas Users API Delete a user login
  x-api-slug: instructure-canvas-users-api
  description: Delete a user login.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/logins/id
  tags: Users,User,Id,Logins,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idloginsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idloginsid-delete-openapi.md
- name: Instructure Canvas Users API List Missing Submissions
  x-api-slug: instructure-canvas-users-api
  description: List missing submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/missing_submissions
  tags: Users,User,Id,Missing,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idmissing-submissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idmissing-submissions-get-openapi.md
- name: Instructure Canvas Users API List observees
  x-api-slug: instructure-canvas-users-api
  description: List observees.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees
  tags: Users,User,Id,Observees
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobservees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobservees-get-openapi.md
- name: Instructure Canvas Users API Add an observee with credentials
  x-api-slug: instructure-canvas-users-api
  description: Add an observee with credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees
  tags: Users,User,Id,Observees
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobservees-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobservees-post-openapi.md
- name: Instructure Canvas Users API Remove an observee
  x-api-slug: instructure-canvas-users-api
  description: Remove an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-delete-openapi.md
- name: Instructure Canvas Users API Show an observee
  x-api-slug: instructure-canvas-users-api
  description: Show an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-get-openapi.md
- name: Instructure Canvas Users API Add an observee
  x-api-slug: instructure-canvas-users-api
  description: Add an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idobserveesobservee-id-put-openapi.md
- name: Instructure Canvas Users API List user page views
  x-api-slug: instructure-canvas-users-api
  description: List user page views.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/page_views
  tags: Users,User,Id,Page,Views
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idpage-views-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idpage-views-get-openapi.md
- name: Instructure Canvas Users API Get user profile
  x-api-slug: instructure-canvas-users-api
  description: Get user profile.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/profile
  tags: Users,User,Id,Profile
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idprofile-get-openapi.md
- name: Instructure Canvas Users API Remove usage rights
  x-api-slug: instructure-canvas-users-api
  description: Remove usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/usage_rights
  tags: Users,User,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idusage-rights-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idusage-rights-delete-openapi.md
- name: Instructure Canvas Users API Set usage rights
  x-api-slug: instructure-canvas-users-api
  description: Set usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/usage_rights
  tags: Users,User,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idusage-rights-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/usersuser-idusage-rights-put-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---