{
  "info": {
    "name": "Plentymarkets List item set components of an item set",
    "_postman_id": "68746f87-7516-47b2-be9e-6d8e368b96f5",
    "description": "Lists the item set components of an item set. The ID of the item set must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "9311f6f3-4d37-4c08-bbb1-d1df7a20a4e7",
          "name": "getRestItemSetsSetComponents",
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
            "description": "Lists the item set components of an item set. The ID of the item set must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b5030cd-340e-4378-9778-54e89be16984"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "68482dda-9af5-4e15-be02-3f8052f1428c",
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
              "id": "ade6b322-0813-4596-9b42-0a42d3a1e939"
            }
          ]
        }
      ]
    }
  ]
}