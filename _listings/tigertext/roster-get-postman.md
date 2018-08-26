{
  "info": {
    "name": "Tiger Connect Roster API Get the recent conversation list for a user. As new messages are sent and received, the roster is updated with those conversations.",
    "_postman_id": "b6dfebfc-a8d3-40b0-9eda-f8924db14242",
    "description": "Get the recent conversation list for a user. As new messages are sent and received, the roster is updated with those conversations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Roster",
      "item": [
        {
          "id": "3385364e-2c0c-4ed0-8b8a-bebbc3402017",
          "name": "getRoster",
          "request": {
            "url": "http://developer.tigertext.me/v2/roster/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the recent conversation list for a user. As new messages are sent and received, the roster is updated with those conversations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54b039ab-f4b5-4820-9581-66c07280e074"
            }
          ]
        }
      ]
    }
  ]
}