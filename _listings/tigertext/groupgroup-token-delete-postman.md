{
  "info": {
    "name": "Tiger Connect Group API Delete a group. If the group has already been deleted, no error is reported.",
    "_postman_id": "4cb653f2-5539-440c-ac7d-1356909600e5",
    "description": "Delete a group. If the group has already been deleted, no error is reported.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "00bcf987-a20e-43da-ae45-3446e6bbbbc9",
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
          "id": "519a3a59-682d-4686-bee4-5d30c50e0adb"
        }
      ]
    },
    {
      "id": "5bbe27c7-cc90-4a42-b67e-834085d17fbc",
      "name": "deleteGroup",
      "request": {
        "url": {
          "protocol": "http",
          "host": "developer.tigertext.me",
          "path": [
            "v2",
            "group/:group_token/"
          ],
          "variable": [
            {
              "id": "group_token",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "DELETE",
        "body": {
          "mode": "raw"
        },
        "description": "Delete a group. If the group has already been deleted, no error is reported."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c8d572cb-c965-4a3f-99cf-be3e893670d6"
        }
      ]
    }
  ]
}