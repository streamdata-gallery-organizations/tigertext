{
  "info": {
    "name": "Tiger Connect Message API Update the status of a message or several messages.",
    "_postman_id": "c3323ba1-42de-4b38-b447-9bb3f804a41b",
    "description": "Update the status of a message or several messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "27d6042f-a20a-40e2-846f-9d0fd78a9778",
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
              "id": "dc30eb6f-3d54-4f26-8c37-fa83e2de92d2"
            }
          ]
        },
        {
          "id": "41d8fb47-ce55-4b8e-8e6e-b5181019dc98",
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
              "id": "e45aa094-c473-4fb3-9006-b71d72ebd0ef"
            }
          ]
        }
      ]
    }
  ]
}