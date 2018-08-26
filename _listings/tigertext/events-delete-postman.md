{
  "info": {
    "name": "Tiger Connect Events API Drop the events connections.",
    "_postman_id": "d3f822a3-916f-414b-bb23-d46f37a5e10a",
    "description": "Drop the events connections.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "7fada175-6452-40af-900a-44063c31116c",
          "name": "dropConnect",
          "request": {
            "url": "http://developer.tigertext.me/v2/events/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Drop the events connections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06a0ca7d-0153-4b6e-bb5c-817458a757d3"
            }
          ]
        }
      ]
    }
  ]
}