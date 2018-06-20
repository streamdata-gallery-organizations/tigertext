{
  "info": {
    "name": "Tiger Connect Message API Notify a recipient that the User is no longer typing in a conversation.",
    "_postman_id": "8e68d04c-87c1-4d06-b603-b71fb891d2a5",
    "description": "Notify a recipient that the User is no longer typing in a conversation. The recipient is either another User or Group using address encoding.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "28edea9e-63b3-4171-9a34-12dd537d66a2",
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
              "id": "85578632-6c52-4fd5-9ae3-e269cedbe401"
            }
          ]
        }
      ]
    }
  ]
}