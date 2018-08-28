{
  "info": {
    "name": "Plentymarkets List dates of an order item",
    "_postman_id": "4f916205-bb2b-4e51-a9a8-9ec697999c6a",
    "description": "Lists the dates of an order item. The ID of the order item must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "1bacb7ea-10ad-4f3c-bc8e-3f429af97444",
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
              "id": "87d6c052-b514-49ae-99b9-14cb41514728"
            }
          ]
        }
      ]
    }
  ]
}