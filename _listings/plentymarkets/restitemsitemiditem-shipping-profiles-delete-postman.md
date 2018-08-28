{
  "info": {
    "name": "Plentymarkets Deactivate shipping profiles of an item",
    "_postman_id": "95864c0e-bb65-44db-a278-2dc9345fc8ce",
    "description": "Deactivates all shipping profiles of an item. The ID of the item must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deactivate",
      "item": [
        {
          "id": "ce7f4cf8-3a68-42ed-a5f3-2b6731cc7513",
          "name": "deleteRestCategoriesClients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/categories/:id/clients"
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
            "description": "Deactivate availability for clients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46549b42-05f1-446c-8aaf-0721a410b799"
            }
          ]
        },
        {
          "id": "0580567e-32c2-46ae-bf38-a42ae8cfeeb1",
          "name": "deleteRestItemsBarcodesBarcodeReferrerReferrer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/barcodes/:barcodeId/referrer/:referrerId"
              ],
              "variable": [
                {
                  "id": "barcodeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "referrerId",
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
            "description": "Deactivate a referrer for a barcode. The ID of the barcode and the ID of the referrer must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a833a2fc-39e4-4d91-9822-44b674398530"
            }
          ]
        },
        {
          "id": "ff580d89-687f-4685-a856-edc8573a8246",
          "name": "deleteRestItemsSalesPricesAccountsAccounttypeAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/accounts/:accountType/:accountId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "accountType",
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
            "description": "Deactivates a referrer account for a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49c67025-e5ce-4aac-b5cc-59c08318b7cc"
            }
          ]
        },
        {
          "id": "930954d0-81ae-4f76-acb4-c0b714cafd6e",
          "name": "deleteRestItemsSalesPricesCountriesCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/countries/:countryId"
              ],
              "variable": [
                {
                  "id": "countryId",
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
            "description": "Deactivates a country for a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a529b55-ee89-47d9-ad5c-52a0d091c671"
            }
          ]
        },
        {
          "id": "f5f226d4-7078-415a-82be-7c49c17cd917",
          "name": "deleteRestItemsSalesPricesCurrenciesCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/currencies/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
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
            "description": "Deactivate a currency for a sales price. The ID of the sales price and the ISO code of the currency must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bbae7e3-e0fe-4b17-880c-9a24bd1c71fb"
            }
          ]
        },
        {
          "id": "a8247b73-3516-443b-9709-3cc7065656b7",
          "name": "deleteRestItemsSalesPricesOnlineStoresWebstore",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/online_stores/:webstoreId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webstoreId",
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
            "description": "Deactivates a client (store) for a sales price. The ID of the sales price and the ID of the client (store) must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "336d3756-84a8-41e8-beeb-eabb7dab97a0"
            }
          ]
        },
        {
          "id": "d30460a0-02a3-496b-8d92-520d63e95bc8",
          "name": "deleteRestItemsItemItemShippingProfiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:itemId/item_shipping_profiles"
              ],
              "variable": [
                {
                  "id": "itemId",
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
            "description": "Deactivates all shipping profiles of an item. The ID of the item must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58c84f56-7a9c-4ad7-b60d-14e5a830786f"
            }
          ]
        }
      ]
    }
  ]
}