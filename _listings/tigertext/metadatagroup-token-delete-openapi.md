---
swagger: "2.0"
x-collection-name: TigerText
x-complete: 0
info:
  title: Tiger Connect Metadata API Clears the metadata for a User or Group based
    on address encoding.
  description: Clears the metadata for a User or Group based on address encoding.
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
  /metadata/{group_token}/:
    delete:
      summary: Clears the metadata for a User or Group based on address encoding.
      description: Clears the metadata for a User or Group based on address encoding.
      operationId: deleteMetadata
      x-api-path-slug: metadatagroup-token-delete
      parameters:
      - in: path
        name: group_token
        description: The group token
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Group
      - Token
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