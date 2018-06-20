{
  "info": {
    "name": "Tiger Connect Group API Add members to a group.",
    "_postman_id": "cb7620c2-74f3-4a1a-b610-0bc56866d569",
    "description": "Add members to a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "ab927497-2795-4444-a83d-332234f0855d",
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
          "id": "2cdd6548-c53a-4789-ba23-d433fdb714da"
        }
      ]
    },
    {
      "id": "2ebd7bd0-e860-41ac-b354-06651a95e86a",
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
          "id": "e8134375-a12c-457c-82cd-98f422d1d20c"
        }
      ]
    },
    {
      "id": "32f4ef5c-69c1-43f5-aeda-20d9f693b497",
      "name": "addGroupMember",
      "request": {
        "url": {
          "protocol": "http",
          "host": "developer.tigertext.me",
          "path": [
            "v2",
            "group/:group_token/members/"
          ],
          "variable": [
            {
              "id": "group_token",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "POST",
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "members",
              "value": "{}",
              "disabled": false,
              "description": "A list of members to add to a group using user address encoding"
            }
          ]
        },
        "description": "Add members to a group."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "354859f0-67d7-4f8c-ba37-096162be43da"
        }
      ]
    }
  ]
}