---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty List a user's notification rules
  version: 1.0.0
  description: List notification rules of your PagerDuty user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/notification_rules:
    get:
      summary: List a user's notification rules
      description: List notification rules of your PagerDuty user.
      operationId: list-notification-rules-of-your-pagerduty-user
      x-api-path-slug: usersidnotification-rules-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Notification Rules
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