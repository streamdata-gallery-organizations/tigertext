{
  "info": {
    "name": "Tiger Connect Metadata API Get the metadata for a User or Group based on address encoding.",
    "_postman_id": "0ff188d0-f337-4ed8-bb40-c1645d7f1cbf",
    "description": "Get the metadata for a User or Group based on address encoding.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Metadata",
      "item": [
        {
          "id": "e2a43d80-278d-435e-831b-1b28c8857cfc",
          "name": "getMetadata",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the metadata for a User or Group based on address encoding."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff3f90d7-2f43-4de1-a733-af2534e7ea8d"
            }
          ]
        },
        {
          "id": "19017456-c5f2-485b-9c2f-b0efa4070eb0",
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
              "id": "842ead61-b036-4bd1-ae0e-09862671498b"
            }
          ]
        }
      ]
    }
  ]
}