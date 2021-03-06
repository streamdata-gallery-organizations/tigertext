---
swagger: "2.0"
x-collection-name: TigerText
x-complete: 0
info:
  title: Tiger Connect Group API Create a new group.
  description: Create a new group.
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
  /events/:
    delete:
      summary: Drop the events connections.
      description: Drop the events connections.
      operationId: dropConnect
      x-api-path-slug: events-delete
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: Opens a SSE event stream.
      description: Opens a SSE event stream. The various Event Types are listed below.
      operationId: createEvents
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /group/:
    post:
      summary: Create a new group.
      description: Create a new group.
      operationId: createNewGroup
      x-api-path-slug: group-post
      parameters:
      - in: query
        name: avatar
        description: Binary data to use for the groups avatar
      - in: formData
        name: members
        description: The members to add to the group encoded using user address encoding
      - in: formData
        name: name
        description: The group name
      - in: formData
        name: replay_history
        description: A boolean value indicating if, when a new member is added to
          the group, it should get the messages sent to the group before that
      - in: formData
        name: TT-X-Organization-Key
        description: The organization in which the user wants to create the group
      responses:
        200:
          description: OK
      tags:
      - ""
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