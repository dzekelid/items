{
  "info": {
    "name": "Plentymarkets Create item set components",
    "_postman_id": "6758f6ad-a004-4759-a64b-ff732fb3e77c",
    "description": "Create item set components.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "59156b76-d89e-44bc-afd2-f2a12cdb7cdb",
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
              "id": "0e68f192-805e-4b5d-b3e7-346896f28529"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "e768989f-d374-4aac-998b-d37758e4905c",
          "name": "postRestItemSetsSetComponents",
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
            "method": "POST",
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
            "description": "Create item set components."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77b351f5-6089-4718-9f45-aed5c1c50331"
            }
          ]
        },
        {
          "id": "cddb48c0-2e64-480e-96fa-6bd78e80cfbd",
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
              "id": "98030b7c-6df5-47f2-87a7-d6136fa7b0fe"
            }
          ]
        }
      ]
    }
  ]
}