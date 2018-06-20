{
  "info": {
    "name": "Tiger Connect Message API Notify a recipient that a particular User is typing in a conversation.",
    "_postman_id": "c9fe4ff1-d407-4c1d-950e-66c6e1cef47f",
    "description": "Notify a recipient that a particular User is typing in a conversation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "5ea87134-e2f5-4ce0-ab75-649be9306f39",
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
              "id": "3681330d-3b85-400f-8548-d66d8194ef8d"
            }
          ]
        },
        {
          "id": "303e26f6-30e2-4637-a079-e0842ae3ea46",
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
              "id": "7afa6c4d-d515-4f54-8466-ae78ee01c147"
            }
          ]
        },
        {
          "id": "c1f361e6-4ffa-49cf-8b19-1a3b735a6e71",
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
              "id": "333ed80c-fb90-41e4-b3d6-b78041cb00a6"
            }
          ]
        }
      ]
    }
  ]
}