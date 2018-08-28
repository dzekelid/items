{
  "info": {
    "name": "Plentymarkets Get a date of an order item",
    "_postman_id": "e3bee76a-4ec6-4a25-bf87-e09c3632e876",
    "description": "Gets a date of an order item. The ID of the date must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "389e5e94-5a0a-4a32-9f72-a984e9a416c4",
          "name": "getRestOrdersItemsOrderitemDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/:orderItemId/dates"
              ],
              "variable": [
                {
                  "id": "orderItemId",
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
            "description": "Lists the dates of an order item. The ID of the order item must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fc72b49-a8d1-4148-a908-ba5dadfa98af"
            }
          ]
        },
        {
          "id": "b52e8fd6-4fe6-465a-9220-1d81bd45b312",
          "name": "getRestOrdersOrderDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/dates"
              ],
              "variable": [
                {
                  "id": "orderId",
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
            "description": "Lists dates of an order. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33ebaad8-995c-48cb-b715-d883ff8f1c2d"
            }
          ]
        },
        {
          "id": "fc5127a3-9fd2-47c0-8ad8-e9c37ef0a1b4",
          "name": "getRestOrdersDatesTypes",
          "request": {
            "url": "http://example.com/rest/orders/dates/types",
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
            "description": "List order date types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64bd1695-3d9b-4fa4-aba7-ef48709c43bd"
            }
          ]
        },
        {
          "id": "00d0a097-e3c7-443d-8f62-f8c2e284efed",
          "name": "getRestOrdersDatesTypesTypeNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId/names"
              ],
              "variable": [
                {
                  "id": "typeId",
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
            "description": "Lists names in all languages available of an order date type. The ID of the date type must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faefc776-7722-430a-ad63-42e0b8908abc"
            }
          ]
        }
      ]
    },
    {
      "name": "Find",
      "item": [
        {
          "id": "da2cb7e4-fff6-4f45-811f-15c846017f6e",
          "name": "getRestOrdersDatesTypesType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId"
              ],
              "variable": [
                {
                  "id": "typeId",
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
            "description": "Find an order date type by it's id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f861f732-a4b8-455f-85d0-fda28cc757a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Name",
      "item": [
        {
          "id": "b3b1e26f-a558-404b-97b1-f31df5979076",
          "name": "getRestOrdersDatesTypesTypeNamesLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId/names/:lang"
              ],
              "variable": [
                {
                  "id": "lang",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "typeId",
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
            "description": "Gets a name of an order date type. The ID of the date type and the language of the name must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18869db2-ef3d-4988-b59a-22f348c9e86d"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "124020a2-c4af-4649-b48a-d8d8f3016f91",
          "name": "getRestOrdersItemsDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/dates/:id"
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
            "description": "Gets a date of an order item. The ID of the date must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbccc287-bf62-4ff6-bfae-8b1ea51aebb3"
            }
          ]
        },
        {
          "id": "43dc71cd-94fe-4872-9b56-cc667865fdef",
          "name": "deleteRestOrdersItemsDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/dates/:id"
              ],
              "variable": [
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
            "description": "Deletes the date from an order item. The ID of the date must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9be44cf-bb1c-456b-8c33-7ac644d21f98"
            }
          ]
        }
      ]
    }
  ]
}