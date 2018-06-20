{
  "info": {
    "name": "Tiger Connect Group API Create a new group.",
    "_postman_id": "ca29e6d1-1143-4ea6-8f39-12a26c0a23db",
    "description": "Create a new group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "4f74d07c-8f24-4980-86b5-60faacef8bcf",
      "name": "createNewGroup",
      "request": {
        "url": "http://developer.tigertext.me/v2/group/?avatar=%7B%7D",
        "method": "POST",
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "members",
              "value": "{}",
              "disabled": false,
              "description": "The members to add to the group encoded using user address encoding"
            },
            {
              "key": "name",
              "value": "{}",
              "disabled": false,
              "description": "The group name"
            },
            {
              "key": "replay_history",
              "value": "{}",
              "disabled": false,
              "description": "A boolean value indicating if, when a new member is added to the group, it should get the messages sent to the group before that"
            },
            {
              "key": "TT-X-Organization-Key",
              "value": "{}",
              "disabled": false,
              "description": "The organization in which the user wants to create the group"
            }
          ]
        },
        "description": "Create a new group."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5d4ba7a7-4400-4bfd-824d-bedc266529c0"
        }
      ]
    }
  ]
}