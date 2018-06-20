---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Get single user
  description: Get single user.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/analytics/users/student_id/activity:
    get:
      summary: Get user-in-a-course-level participation data
      description: Get user-in-a-course-level participation data.
      operationId: get-userinacourselevel-participation-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idactivity-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Activity
  /courses/{course_id}/analytics/users/student_id/assignments:
    get:
      summary: Get user-in-a-course-level assignment data
      description: Get user-in-a-course-level assignment data.
      operationId: get-userinacourselevel-assignment-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Assignments
  /courses/{course_id}/analytics/users/student_id/communication:
    get:
      summary: Get user-in-a-course-level messaging data
      description: Get user-in-a-course-level messaging data.
      operationId: get-userinacourselevel-messaging-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idcommunication-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Communication
  /courses/{course_id}/quizzes/id/submission_users/message:
    post:
      summary: Send a message to unsubmitted or submitted users for the quiz
      description: Send a message to unsubmitted or submitted users for the quiz.
      operationId: send-a-message-to-unsubmitted-or-submitted-users-for-the-quiz
      x-api-path-slug: coursescourse-idquizzesidsubmission-usersmessage-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
      - Submission
      - Users
      - Message
  /courses/{course_id}/search_users:
    get:
      summary: List users in course
      description: List users in course.
      operationId: list-users-in-course
      x-api-path-slug: coursescourse-idsearch-users-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return users enrolled with the specifiedncourse-level
          role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_state[]
        description: When set, only return users where the enrollment workflow state
          is of onenof the given types
      - in: query
        name: enrollment_type[]
        description: When set, only return users where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cemailu201d: Optional user email'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: user_id
        description: If included, the user will be queried and if the user is part
          of the usersnset, the page parameter will be modified so that the page containingnuser_id
          will be returned
      - in: query
        name: user_ids[]
        description: If included, the course users set will only include users with
          IDsnspecified by the param
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Search
      - Users
  /courses/{course_id}/users:
    get:
      summary: List users in course
      description: List users in course.
      operationId: list-users-in-course
      x-api-path-slug: coursescourse-idusers-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return users enrolled with the specifiedncourse-level
          role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_state[]
        description: When set, only return users where the enrollment workflow state
          is of onenof the given types
      - in: query
        name: enrollment_type[]
        description: When set, only return users where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cemailu201d: Optional user email'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: user_id
        description: If included, the user will be queried and if the user is part
          of the usersnset, the page parameter will be modified so that the page containingnuser_id
          will be returned
      - in: query
        name: user_ids[]
        description: If included, the course users set will only include users with
          IDsnspecified by the param
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Users
  /courses/{course_id}/users/id:
    get:
      summary: Get single user
      description: Get single user.
      operationId: get-single-user
      x-api-path-slug: coursescourse-idusersid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Users
      - Id
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