---
swagger: "2.0"
x-collection-name: TigerText
x-complete: 1
info:
  title: Tiger Connect User API
  description: the-user-system-for-tigerconnect-messaging-platform-
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
  /user/{user_address}/:
    get:
      summary: Get information about users using their user address encoding.
      description: Get information about users using their user address encoding.
      operationId: getUser
      x-api-path-slug: useruser-address-get
      parameters:
      - in: query
        name: TT-X-Organization-Key
        description: The organization for which to show the users organization-bound
          fields (i
      - in: path
        name: user_address
        description: The user address
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Address
---