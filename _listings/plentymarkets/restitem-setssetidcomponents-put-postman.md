{
  "info": {
    "name": "Plentymarkets Update item set components",
    "_postman_id": "739d9ed6-bcf5-47b5-bb1d-66fca25bcdca",
    "description": "Update item set components.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "4e56e2e3-96a1-4fa5-a3c9-79071b182630",
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
              "id": "41b7204c-1bd8-4200-9eee-f2b699c8b5db"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "234376d1-360b-434c-8f4b-e6594c42cee0",
          "name": "putRestItemSetsSetComponents",
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
            "method": "PUT",
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
            "description": "Update item set components."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af680751-0d97-4408-a08c-b162ac97c70f"
            }
          ]
        },
        {
          "id": "5851c133-0c6a-42c4-85c4-44367d2ee3a0",
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
              "id": "57b2be2b-89f6-41af-8a6b-6f1a8373855a"
            }
          ]
        },
        {
          "id": "d19570d8-c238-4ac3-89c3-fc6c923168ca",
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
              "id": "51fd97f7-22c6-496b-b8bf-ea4002bb842d"
            }
          ]
        }
      ]
    }
  ]
}