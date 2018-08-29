---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Send a message to unsubmitted or submitted
    users for the quiz
  description: Send a message to unsubmitted or submitted users for the quiz.
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