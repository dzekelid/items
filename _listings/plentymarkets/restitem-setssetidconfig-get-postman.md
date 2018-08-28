{
  "info": {
    "name": "Plentymarkets Get the item set configuration of an item set",
    "_postman_id": "fc796e12-9d18-4e34-b721-f77a9043b68a",
    "description": "Get the item set configuration of an item set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "27c16e3d-7d10-4857-9253-5c5a669d571d",
          "name": "getRestAccountingLocationsRevenueAccountConfigurations",
          "request": {
            "url": "http://example.com/rest/accounting/locations/revenue_account_configurations?itemsPerPage=%7B%7D&page=%7B%7D",
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
            "description": "Lists revenue account configurations of a system. The revenue accounts are returned as paginated result. By default 50 revenue accounts are on one page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5aadc8d8-fb7b-4eb7-bd1e-d80e47859bce"
            }
          ]
        },
        {
          "id": "29309f66-9892-4512-a5e4-70ad6acdb017",
          "name": "getRestVat",
          "request": {
            "url": "http://example.com/rest/vat?columns=%7B%7D&itemsPerPage=%7B%7D&page=%7B%7D&with=%7B%7D",
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
            "description": "Lists the VAT configurations for the given filter. Possible filters are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code> and <code>startedAt</code>."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82351d5b-83a0-4f95-8da2-7207b937ca2d"
            }
          ]
        },
        {
          "id": "5a37950a-f3e7-4ca6-9ad1-1e06f4274508",
          "name": "getRestVatLocationsLocation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/vat/locations/:locationId"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "with",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Lists the VAT configurations for all countries of one accounting location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4719b0c-b90d-4854-9e68-951d4ccb3251"
            }
          ]
        }
      ]
    },
    {
      "name": "Revenue",
      "item": [
        {
          "id": "25ffdd65-5e8a-455e-a592-14dc44527397",
          "name": "getRestAccountingLocationsLocationCountriesCountryRevenueAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/countries/:countryId/revenue_accounts"
              ],
              "variable": [
                {
                  "id": "countryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "locationId",
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
            "description": "Get the revenue account configuration of a country. The ID of the accounting location that the country is associated with as well as the ID of the country must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd3b3c3-6129-4acc-9ee9-cb26ecb502a4"
            }
          ]
        },
        {
          "id": "224e9f69-1b07-446c-810a-504aeeaa1833",
          "name": "getRestAccountingLocationsLocationRevenueAccountConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/revenue_account_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets the revenue account configuration of an accounting location. A revenue account location configuration contains several revenue accounts. The ID of the accounting location has to be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9ef1439-0c0e-4c7f-8ecb-53d938bb100c"
            }
          ]
        }
      ]
    },
    {
      "name": "Debtor",
      "item": [
        {
          "id": "a7dc5049-52a5-4be3-aafc-92354f7c9140",
          "name": "getRestAccountingLocationsLocationDebtorAccountConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/debtor_account_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets the debtor account configuration of an accounting location. The ID of the accounting location has to be specified. The debtor account configuration can contain one standard debtor account only or e.g. several accounts for each country of delivery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a86254a2-6397-4651-991d-9d3d9b59e90b"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "55408bb2-8d56-4e3e-aa86-9c65c23864f7",
          "name": "getRestAccountingLocationsLocationAddingKeyConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/posting_key_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets a posting key configuration of an accounting location. The ID of the accounting location has to be specified. The posting key configuration can contain up to 4 posting keys."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e15bf232-7f61-4542-9729-4fd18d2f7846"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "c3559049-b37b-4b85-9139-620f92fa7c35",
          "name": "getRestItemSetsSetConfig",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/config"
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
            "description": "Get the item set configuration of an item set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7f0022c-caec-4f8a-89c6-1ad014c3617e"
            }
          ]
        }
      ]
    }
  ]
}