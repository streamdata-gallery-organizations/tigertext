---
swagger: "2.0"
x-collection-name: TigerText
x-complete: 0
info:
  title: Tiger Connect Message API Get information about a message
  description: Get information about a message
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
  /message/:
    post:
      summary: Send a message to a User or Group.
      description: Send a message to a User or Group. The parameters to be included
        either on the JSON object or the POST body itself. If no recipient is found,
        a new account is created and the message is sent to the associated email or
        phone number if available.
      operationId: sendMessage
      x-api-path-slug: message-post
      parameters:
      - in: formData
        name: body
        description: The message body
      - in: formData
        name: data
        description: A JSON Array of user-defined datum elements, each one with the
          following fields, if no data then this will be empty
      - in: formData
        name: dor
        description: Boolean value indicating that the message will be deleted on
          read
      - in: query
        name: recipient
        description: The recipient User or Group based on address encoding
      - in: formData
        name: recipient_organization
        description: The recipient organization token
      - in: formData
        name: sender_organization
        description: The sender User organization token
      - in: formData
        name: ttl
        description: An integer value with the number of minutes until the message
          expires
      responses:
        200:
          description: OK
      tags:
      - Message
  /message/status/:
    put:
      summary: Update the status of a message or several messages.
      description: Update the status of a message or several messages.
      operationId: updateMessageStatus
      x-api-path-slug: messagestatus-put
      parameters:
      - in: formData
        name: delivered
        description: A list of message tokens to set status to Delivered
      - in: formData
        name: read
        description: A list of message tokens to set status to Read
      responses:
        200:
          description: OK
      tags:
      - Message
      - Status
  /message/typing/:
    get:
      summary: Notify a recipient that a particular User is typing in a conversation.
      description: Notify a recipient that a particular User is typing in a conversation.
      operationId: typingMessage
      x-api-path-slug: messagetyping-get
      parameters:
      - in: query
        name: recipient
        description: The recipient is either another User or Group using address encoding
      responses:
        200:
          description: OK
      tags:
      - Message
      - Typing
  /message/typing/{recipient_address}/:
    delete:
      summary: Notify a recipient that the User is no longer typing in a conversation.
      description: Notify a recipient that the User is no longer typing in a conversation.
        The recipient is either another User or Group using address encoding.
      operationId: deleteMessageTyping
      x-api-path-slug: messagetypingrecipient-address-delete
      parameters:
      - in: path
        name: recipient_address
        description: The recipient address
      responses:
        200:
          description: OK
      tags:
      - Message
      - Typing
      - Recipient
      - Address
  /message/{message_token}/:
    delete:
      summary: Recalls the message with the following message token.
      description: Recalls the message with the following message token. If the message
        was already recalled, no error is reported.
      operationId: deleteMessage
      x-api-path-slug: messagemessage-token-delete
      parameters:
      - in: path
        name: message_token
        description: The message token
      responses:
        200:
          description: OK
      tags:
      - Message
      - Message
      - Token
    get:
      summary: Get information about a message
      description: Get information about a message
      operationId: getMessage
      x-api-path-slug: messagemessage-token-get
      parameters:
      - in: path
        name: message_token
        description: The message token
      responses:
        200:
          description: OK
      tags:
      - Message
      - Message
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