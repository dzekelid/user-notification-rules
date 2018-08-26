---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
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
    post:
      summary: Create a user notification rule
      description: Create a new notification rule.
      operationId: create-a-new-notification-rule
      x-api-path-slug: usersidnotification-rules-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: notification_rule
        description: The notification rule to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User Notification Rules
  /users/{id}/notification_rules/{notification_rule_id}:
    get:
      summary: Get a user's notification rule
      description: Get users  notification rules notification rule
      operationId: get-details-about-a-users-notification-rule
      x-api-path-slug: usersidnotification-rulesnotification-rule-id-get
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
    delete:
      summary: Delete a user's notification rule
      description: Delete users  notification rules notification rule
      operationId: remove-a-users-notification-rule
      x-api-path-slug: usersidnotification-rulesnotification-rule-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Notification Rules
    put:
      summary: Update a user's notification rule
      description: Put users  notification rules notification rule
      operationId: update-a-users-notification-rule
      x-api-path-slug: usersidnotification-rulesnotification-rule-id-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: notification_rule
        description: The users notification rule to be updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User Notification Rules
---