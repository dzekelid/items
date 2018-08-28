{
  "info": {
    "name": "Plentymarkets Get an item availability",
    "_postman_id": "fe5156ee-aa71-466a-b155-dc04e302dbe7",
    "description": "Gets an item availability. The ID of the availability must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Item",
      "item": [
        {
          "id": "033802e8-81c9-4edb-b5c7-8b603227612b",
          "name": "getRestAvailabilities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/availabilities/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets an item availability. The ID of the availability must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16802136-f191-4119-9f44-a76fbb856008"
            }
          ]
        }
      ]
    }
  ]
}