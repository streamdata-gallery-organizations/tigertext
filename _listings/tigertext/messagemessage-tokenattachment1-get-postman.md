{
  "info": {
    "name": "Tiger Connect Message API Retrieves the attachment from the message.",
    "_postman_id": "0d5e3c59-7fb3-4f94-bf25-10dccf942361",
    "description": "Retrieves the attachment from the message. Currently we only support one attachment per message. if found. It returns the attached file.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "d9394e5e-42af-484c-ae51-f0724080750f",
          "name": "sendMessage",
          "request": {
            "url": "http://developer.tigertext.me/v2/message/?recipient=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The message body"
                },
                {
                  "key": "data",
                  "value": "{}",
                  "disabled": false,
                  "description": "A JSON Array of user-defined datum elements, each one with the following fields, if no data then this will be empty"
                },
                {
                  "key": "dor",
                  "value": "{}",
                  "disabled": false,
                  "description": "Boolean value indicating that the message will be deleted on read"
                },
                {
                  "key": "recipient_organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The recipient organization token"
                },
                {
                  "key": "sender_organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The sender User organization token"
                },
                {
                  "key": "ttl",
                  "value": "{}",
                  "disabled": false,
                  "description": "An integer value with the number of minutes until the message expires"
                }
              ]
            },
            "description": "Send a message to a User or Group. The parameters to be included either on the JSON object or the POST body itself. If no recipient is found, a new account is created and the message is sent to the associated email or phone number if available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d13affab-b88a-497f-bd5b-07bfbf8ffb34"
            }
          ]
        },
        {
          "id": "0f8e95c6-5e05-4f38-8ecb-16aa664127c9",
          "name": "updateMessageStatus",
          "request": {
            "url": "http://developer.tigertext.me/v2/message/status/",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "delivered",
                  "value": "{}",
                  "disabled": false,
                  "description": "A list of message tokens to set status to Delivered"
                },
                {
                  "key": "read",
                  "value": "{}",
                  "disabled": false,
                  "description": "A list of message tokens to set status to Read"
                }
              ]
            },
            "description": "Update the status of a message or several messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89cbbfae-6fca-47e6-8fd3-93615a012bae"
            }
          ]
        },
        {
          "id": "176cfe45-3b83-42ef-9c9b-902cba73f96a",
          "name": "typingMessage",
          "request": {
            "url": "http://developer.tigertext.me/v2/message/typing/?recipient=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Notify a recipient that a particular User is typing in a conversation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36e0de4-6886-4f35-9202-71eab806ec69"
            }
          ]
        },
        {
          "id": "5483e85e-0fed-4d86-8f1c-43c83524e0dd",
          "name": "deleteMessageTyping",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "message/typing/:recipient_address/"
              ],
              "variable": [
                {
                  "id": "recipient_address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Notify a recipient that the User is no longer typing in a conversation. The recipient is either another User or Group using address encoding."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "460e8e11-eef5-4514-83f6-c41e4463b523"
            }
          ]
        },
        {
          "id": "208932f2-4d96-4041-802b-c34364fc214d",
          "name": "getMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "message/:message_token/"
              ],
              "variable": [
                {
                  "id": "message_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a message"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa776423-a8d2-498f-a0c4-a3fbbd9c5859"
            }
          ]
        },
        {
          "id": "404d87e3-f4ea-45bd-b8bf-44435b493629",
          "name": "deleteMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "message/:message_token/"
              ],
              "variable": [
                {
                  "id": "message_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Recalls the message with the following message token. If the message was already recalled, no error is reported."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aab1ec1b-fd12-442e-b458-1e19261faad9"
            }
          ]
        },
        {
          "id": "5d5cc2b2-035e-4f3b-808c-9654981dfc32",
          "name": "getMessageAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "message/:message_token/attachment/1/"
              ],
              "variable": [
                {
                  "id": "message_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attachment from the message. Currently we only support one attachment per message. if found. It returns the attached file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e95207d-d5a3-4e31-979c-81adc1a28bd1"
            }
          ]
        }
      ]
    }
  ]
}