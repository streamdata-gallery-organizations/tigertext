---
name: TigerText
x-slug: tigertext
description: TigerText is a multi-platform, secure, real-time messaging application
  for the enterprise that allows text messages to be deleted from both the senders
  and the receivers phones after expiration, which could be a set period of time or
  after reading. The messages cannot be saved, copied or forwarded by recipients.
  TigerText does this by storing the message on a company server, not the receiving
  and sending device, and deleting when the expiration conditions are met.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: TigerText
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/apis.md
specificationVersion: "0.14"
apis:
- name: Tiger Connect Events API Drop the events connections.
  x-api-slug: tiger-connect-events-api
  description: Drop the events connections.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///events/
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/events-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/events-delete-openapi.md
- name: Tiger Connect Events API Opens a SSE event stream.
  x-api-slug: tiger-connect-events-api
  description: Opens a SSE event stream. The various Event Types are listed below.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///events/
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/events-get-openapi.md
- name: Tiger Connect Events API
  x-api-slug: tiger-connect-events-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
- name: Tiger Connect Group API Create a new group.
  x-api-slug: tiger-connect-group-api
  description: Create a new group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///group/
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/group-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/group-post-openapi.md
- name: Tiger Connect Group API Delete a group. If the group has already been deleted,
    no error is reported.
  x-api-slug: tiger-connect-group-api
  description: Delete a group. If the group has already been deleted, no error is
    reported.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///group/{group_token}/
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-token-delete-openapi.md
- name: Tiger Connect Group API Add members to a group.
  x-api-slug: tiger-connect-group-api
  description: Add members to a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///group/{group_token}/members/
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-tokenmembers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-tokenmembers-post-openapi.md
- name: Tiger Connect Group API Remove members from a group.
  x-api-slug: tiger-connect-group-api
  description: Remove members from a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///group/{group_token}/members/remove/
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-tokenmembersremove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/groupgroup-tokenmembersremove-post-openapi.md
- name: Tiger Connect Group API
  x-api-slug: tiger-connect-group-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
- name: Tiger Connect Message API Send a message to a User or Group.
  x-api-slug: tiger-connect-message-api
  description: Send a message to a User or Group. The parameters to be included either
    on the JSON object or the POST body itself. If no recipient is found, a new account
    is created and the message is sent to the associated email or phone number if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/
  tags: Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/message-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/message-post-openapi.md
- name: Tiger Connect Message API Update the status of a message or several messages.
  x-api-slug: tiger-connect-message-api
  description: Update the status of a message or several messages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/status/
  tags: Message,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagestatus-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagestatus-put-openapi.md
- name: Tiger Connect Message API Notify a recipient that a particular User is typing
    in a conversation.
  x-api-slug: tiger-connect-message-api
  description: Notify a recipient that a particular User is typing in a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/typing/
  tags: Message,Typing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagetyping-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagetyping-get-openapi.md
- name: Tiger Connect Message API Notify a recipient that the User is no longer typing
    in a conversation.
  x-api-slug: tiger-connect-message-api
  description: Notify a recipient that the User is no longer typing in a conversation.
    The recipient is either another User or Group using address encoding.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/typing/{recipient_address}/
  tags: Message,Typing,Recipient,Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagetypingrecipient-address-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagetypingrecipient-address-delete-openapi.md
- name: Tiger Connect Message API Recalls the message with the following message token.
  x-api-slug: tiger-connect-message-api
  description: Recalls the message with the following message token. If the message
    was already recalled, no error is reported.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/{message_token}/
  tags: Message,Message,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-token-delete-openapi.md
- name: Tiger Connect Message API Get information about a message
  x-api-slug: tiger-connect-message-api
  description: Get information about a message
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/{message_token}/
  tags: Message,Message,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-token-get-openapi.md
- name: Tiger Connect Message API Retrieves the attachment from the message.
  x-api-slug: tiger-connect-message-api
  description: Retrieves the attachment from the message. Currently we only support
    one attachment per message. if found. It returns the attached file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/{message_token}/attachment/1/
  tags: Message,Message,Token,Attachment,1
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-tokenattachment1-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-tokenattachment1-get-openapi.md
- name: Tiger Connect Message API Forward the message to the following User or Group.
  x-api-slug: tiger-connect-message-api
  description: Forward the message to the following User or Group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///message/{message_token}/forward/
  tags: Message,Message,Token,Forward
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-tokenforward-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/messagemessage-tokenforward-post-openapi.md
- name: Tiger Connect Message API
  x-api-slug: tiger-connect-message-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
- name: Tiger Connect Metadata API Clears the metadata for a User or Group based on
    address encoding.
  x-api-slug: tiger-connect-metadata-api
  description: Clears the metadata for a User or Group based on address encoding.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///metadata/{group_token}/
  tags: Metadata,Group,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/metadatagroup-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/metadatagroup-token-delete-openapi.md
- name: Tiger Connect Metadata API Get the metadata for a User or Group based on address
    encoding.
  x-api-slug: tiger-connect-metadata-api
  description: Get the metadata for a User or Group based on address encoding.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///metadata/{group_token}/
  tags: Metadata,Group,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/metadatagroup-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/metadatagroup-token-get-openapi.md
- name: Tiger Connect Metadata API Adds metadata for a User or Group based on address
    encoding
  x-api-slug: tiger-connect-metadata-api
  description: Adds metadata for a User or Group based on address encoding
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///metadata/{group_token}/
  tags: Metadata,Group,Token
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/metadatagroup-token-post-openapi.md
- name: Tiger Connect Metadata API
  x-api-slug: tiger-connect-metadata-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
- name: Tiger Connect Roster API Get the recent conversation list for a user. As new
    messages are sent and received, the roster is updated with those conversations.
  x-api-slug: tiger-connect-roster-api
  description: Get the recent conversation list for a user. As new messages are sent
    and received, the roster is updated with those conversations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///roster/
  tags: Roster
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/roster-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/roster-get-openapi.md
- name: Tiger Connect Roster API Remove a conversation from the recent conversation
    list.
  x-api-slug: tiger-connect-roster-api
  description: Remove a conversation from the recent conversation list. For conversations
    that are with another User, all messages are deleted. For conversations with a
    group, the User leaves the group and is no longer receives subsequent group messages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///roster/{user_address}/
  tags: Roster,User,Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/rosteruser-address-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/rosteruser-address-delete-openapi.md
- name: Tiger Connect Roster API
  x-api-slug: tiger-connect-roster-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
- name: Tiger Connect User API Get information about users using their user address
    encoding.
  x-api-slug: tiger-connect-user-api
  description: Get information about users using their user address encoding.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2///user/{user_address}/
  tags: User,User,Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/useruser-address-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/useruser-address-get-openapi.md
- name: Tiger Connect User API
  x-api-slug: tiger-connect-user-api
  description: TigerText is a multi-platform, secure, real-time messaging application
    for the enterprise that allows text messages to be deleted from both the senders
    and the receivers phones after expiration, which could be a set period of time
    or after reading. The messages cannot be saved, copied or forwarded by recipients.
    TigerText does this by storing the message on a company server, not the receiving
    and sending device, and deleting when the expiration conditions are met.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tigertext-logo.png
  humanURL: http://www.tigertext.com/
  baseURL: https://developer.tigertext.me//v2/
  tags: TigerText
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/tigertext/master/_listings/tigertext/openapi.md
x-common:
- type: x-android-sdk
  url: https://developer.tigertext.com/docs/sdk#android-sdk
- type: x-angellist
  url: https://angel.co/tigertext
- type: x-authentication
  url: https://developer.tigertext.com/docs/tigerconnect-basics#authentication
- type: x-base
  url: http://developer.tigertext.me
- type: x-blog
  url: http://www.tigertext.com/blog/
- type: x-case-studies
  url: http://www.tigertext.com/secure-messaging-case-studies
- type: x-compliance
  url: http://www.tigertext.com/compliance-guarantee/
- type: x-contact-form
  url: http://www.tigertext.com/supportform/
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/tigertext
- type: x-developer
  url: https://developer.tigertext.com/
- type: x-documentation
  url: https://developer.tigertext.com/docs/rest-api-reference
- type: x-email
  url: mailto:info@tigertext.com
- type: x-events
  url: http://www.tigertext.com/event/
- type: x-facebook
  url: https://www.facebook.com/TigerText
- type: x-faq
  url: http://www.tigertext.com/faqs/
- type: x-getting-started
  url: https://developer.tigertext.com/docs
- type: x-github
  url: https://github.com/tigertext
- type: x-google-plus
  url: https://plus.google.com/+TigertextApp/posts
- type: x-instagram
  url: https://instagram.com/tigertext/
- type: x-ios-sdk
  url: https://developer.tigertext.com/docs/sdk#ios-sdk
- type: x-javascript-sdk
  url: https://developer.tigertext.com/docs/sdk#web-sdk
- type: x-license
  url: http://reseller.tigertext.com/license/
- type: x-partner-signup
  url: http://reseller.tigertext.com/partner-signup
- type: x-pricing
  url: http://www.tigertext.com/pricing/
- type: x-privacy
  url: http://www.tigertext.com/privacy-policy/
- type: x-reseller-signup
  url: http://reseller.tigertext.com/
- type: x-security
  url: https://developer.tigertext.com/docs/tigerconnect-basics#security-and-compliance
- type: x-selfservice-registration
  url: https://developer.tigertext.com
- type: x-status
  url: http://status.tigertext.com/
- type: x-terms-of-service
  url: http://www.tigertext.com/developer-terms-of-use/
- type: x-terms-of-service
  url: http://www.tigertext.com/developer-terms-of-use
- type: x-twitter
  url: https://twitter.com/tigertext
- type: x-videos
  url: http://reseller.tigertext.com/videos/
- type: x-vimeo
  url: https://vimeo.com/tigertext
- type: x-webinars
  url: http://www.tigertext.com/webinars/
- type: x-website
  url: http://www.tigertext.com/
- type: x-website
  url: http://tigertext.me
- type: x-white-papers
  url: http://www.tigertext.com/white-papers-case-studie
- type: x-wikipedia
  url: http://en.wikipedia.org/wiki/TigerText
- type: x-windows-sdk
  url: https://developer.tigertext.com/docs/sdk#win-sdk
- type: x-youtube
  url: https://www.youtube.com/tigertext
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---