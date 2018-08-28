{
  "info": {
    "name": "Predix Views Delete a related item by id for tags.",
    "_postman_id": "7c9a9415-8df7-4a2f-a580-82ce8ed84312",
    "description": "Delete a related item by id for tags..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Related",
      "item": [
        {
          "id": "acfe6865-bdc1-4ef8-bac1-c5dea33a912d",
          "name": "deleteDecksTagsFk",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "decks/:id/tags/:fk"
              ],
              "variable": [
                {
                  "id": "fk",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Delete a related item by id for tags.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df20404d-1570-4f55-8bca-a2aeeb6365b2"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/v1"
    }
  ]
}