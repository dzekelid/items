{
  "info": {
    "name": "Plentymarkets List basket items",
    "_postman_id": "42be8c51-f255-4f6f-a105-cd0dc01a1410",
    "description": "Lists all items in the shopping cart for the current customer session.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Basket",
      "item": [
        {
          "id": "6f319dd9-738c-4816-8d3d-e2e4cadecd08",
          "name": "getRestBasket",
          "request": {
            "url": "http://example.com/rest/basket",
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
            "description": "Gets the shopping cart for the current customer session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a600561-c647-4843-a13d-c1712970081d"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "ec8dc017-d0ba-45dc-8d5c-47063e4ae7ea",
          "name": "getRestBasketItems",
          "request": {
            "url": "http://example.com/rest/basket/items",
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
            "description": "Lists all items in the shopping cart for the current customer session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72511d57-c647-4da4-8696-0d38f9d6741f"
            }
          ]
        }
      ]
    }
  ]
}