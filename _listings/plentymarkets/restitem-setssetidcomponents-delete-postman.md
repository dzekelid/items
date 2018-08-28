{
  "info": {
    "name": "Plentymarkets Delete item set components",
    "_postman_id": "330bb909-7e75-483b-b68c-49910924d7b1",
    "description": "Delete item set components.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Item",
      "item": [
        {
          "id": "5db1dc7a-512d-495c-93bc-380fc2c65548",
          "name": "deleteRestItemSetsSetComponents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/components"
              ],
              "variable": [
                {
                  "id": "setId",
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
            "description": "Delete item set components."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee98d303-c851-425d-ba24-1f5a45940b07"
            }
          ]
        }
      ]
    }
  ]
}