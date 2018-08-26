---
swagger: "2.0"
x-collection-name: TigerText
x-complete: 0
info:
  title: Tiger Connect Roster API Get the recent conversation list for a user. As
    new messages are sent and received, the roster is updated with those conversations.
  description: Get the recent conversation list for a user. As new messages are sent
    and received, the roster is updated with those conversations.
  termsOfService: http://www.tigertext.com/developer-terms-of-use
  contact:
    name: TigerText
    url: http://www.tigertext.com/supportform/
    email: info@tigertext.com
  version: v2
host: developer.tigertext.me
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /roster/:
    get:
      summary: Get the recent conversation list for a user. As new messages are sent
        and received, the roster is updated with those conversations.
      description: Get the recent conversation list for a user. As new messages are
        sent and received, the roster is updated with those conversations.
      operationId: getRoster
      x-api-path-slug: roster-get
      responses:
        200:
          description: OK
      tags:
      - Roster
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