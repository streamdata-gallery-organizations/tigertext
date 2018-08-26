{
  "info": {
    "name": "Tiger Connect Message API Recalls the message with the following message token.",
    "_postman_id": "dd038375-4238-4615-afbf-3c89fdd9f612",
    "description": "Recalls the message with the following message token. If the message was already recalled, no error is reported.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "149ef43b-d5b2-4524-a760-81def8e439b2",
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
              "id": "5e4ae55c-96ea-4278-8f95-65f274e342cf"
            }
          ]
        },
        {
          "id": "f3b6a015-f085-4288-bd11-8f2cc0ef1e78",
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
              "id": "f10f99dd-85f1-48bf-926a-4978cb3baefc"
            }
          ]
        },
        {
          "id": "5cb17c89-9005-4461-8312-9fa288f8f8bd",
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
              "id": "8e1e6ba8-f435-4721-a00d-2752cdbec554"
            }
          ]
        },
        {
          "id": "81c377b3-43e9-4b2c-a60e-724579e21149",
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
              "id": "a6e35a6e-1948-453b-97e8-7f9fb29b0f71"
            }
          ]
        },
        {
          "id": "98d72e5f-8012-4ab5-bc34-7b0e3bbac0e1",
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
              "id": "3e241c29-b121-4aef-91a2-e6f64bd9409d"
            }
          ]
        }
      ]
    }
  ]
}