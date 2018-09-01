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
  /group/{group_token}/:
    delete:
      summary: Delete a group. If the group has already been deleted, no error is
        reported.
      description: Delete a group. If the group has already been deleted, no error
        is reported.
      operationId: deleteGroup
      x-api-path-slug: groupgroup-token-delete
      parameters:
      - in: path
        name: group_token
        description: The group token
      responses:
        200:
          description: OK
      tags:
      - ""
  /group/{group_token}/members/:
    post:
      summary: Add members to a group.
      description: Add members to a group.
      operationId: addGroupMember
      x-api-path-slug: groupgroup-tokenmembers-post
      parameters:
      - in: path
        name: group_token
        description: The group token
      - in: formData
        name: members
        description: A list of members to add to a group using user address encoding
      responses:
        200:
          description: OK
      tags:
      - ""
  /group/{group_token}/members/remove/:
    post:
      summary: Remove members from a group.
      description: Remove members from a group.
      operationId: removeMemberFromGroup
      x-api-path-slug: groupgroup-tokenmembersremove-post
      parameters:
      - in: path
        name: group_token
        description: The group token
      - in: formData
        name: members
        description: A list of members to remove from a group using address encoding
      responses:
        200:
          description: OK
      tags:
      - ""
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
  /message/{message_token}/attachment/1/:
    get:
      summary: Retrieves the attachment from the message.
      description: Retrieves the attachment from the message. Currently we only support
        one attachment per message. if found. It returns the attached file.
      operationId: getMessageAttachment
      x-api-path-slug: messagemessage-tokenattachment1-get
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
      - Attachment
      - "1"
  /message/{message_token}/forward/:
    post:
      summary: Forward the message to the following User or Group.
      description: Forward the message to the following User or Group.
      operationId: forwardMessage
      x-api-path-slug: messagemessage-tokenforward-post
      parameters:
      - in: path
        name: message_token
        description: The message token
      - in: formData
        name: recipient_organization
        description: The recipient organization token
      - in: formData
        name: recipient_token
        description: The recipient User or Group token based on address encoding
      - in: formData
        name: sender_organization
        description: The sender User organization token
      responses:
        200:
          description: OK
      tags:
      - Message
      - Message
      - Token
      - Forward
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
    get:
      summary: Get the metadata for a User or Group based on address encoding.
      description: Get the metadata for a User or Group based on address encoding.
      operationId: getMetadata
      x-api-path-slug: metadatagroup-token-get
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
    post:
      summary: Adds metadata for a User or Group based on address encoding
      description: Adds metadata for a User or Group based on address encoding
      operationId: addMetadata
      x-api-path-slug: metadatagroup-token-post
      parameters:
      - in: body
        name: body
        description: The metadata in the body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_token
        description: The group token
      - in: query
        name: TT-X-Organization-Key
        description: The organization with which the entity is associated
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Group
      - Token
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