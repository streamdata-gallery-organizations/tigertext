{
  "info": {
    "name": "Tiger Connect Metadata API Clears the metadata for a User or Group based on address encoding.",
    "_postman_id": "84c99417-d82d-45a9-b0e3-20e85c5f750a",
    "description": "Clears the metadata for a User or Group based on address encoding.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Metadata",
      "item": [
        {
          "id": "e763e79b-d906-4947-ba1e-0a0e97344383",
          "name": "deleteMetadata",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "metadata/:group_token/"
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
            "description": "Clears the metadata for a User or Group based on address encoding."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fd2c61f-098b-40f3-8d66-36c6e15026bb"
            }
          ]
        }
      ]
    }
  ]
}