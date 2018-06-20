{
  "info": {
    "name": "Tiger Connect Message API Get information about a message",
    "_postman_id": "f8ff3839-7df2-4f46-886b-76ade88cd83b",
    "description": "Get information about a message",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "a8095d04-f99a-4597-a22f-67be523d086e",
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
              "id": "1c638459-c862-4795-bb09-7b94aed5d2bc"
            }
          ]
        },
        {
          "id": "a4007595-9806-447b-afa9-feb98e342fb5",
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
              "id": "97661a04-df23-4fe1-8cf1-5b6502293922"
            }
          ]
        },
        {
          "id": "575f682d-1d9d-4fe8-a73a-421270ea7f4c",
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
              "id": "34e9ff2c-d86c-447b-a448-29ee3208105d"
            }
          ]
        },
        {
          "id": "680e2ec8-9487-45e8-bfe4-c4c0f1a10262",
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
              "id": "32d34be3-af27-4e7c-bd4b-250c30a1cb57"
            }
          ]
        },
        {
          "id": "1714c1c8-9b19-450d-8b42-fb478b6d0e65",
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
              "id": "0a13e5fb-4eeb-4565-95cd-6e2af87170b0"
            }
          ]
        },
        {
          "id": "cf20cc43-0a4f-4a91-b17a-a1d2d6445522",
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
              "id": "9e753095-7833-4ce4-be47-ed14e7ea7971"
            }
          ]
        }
      ]
    }
  ]
}