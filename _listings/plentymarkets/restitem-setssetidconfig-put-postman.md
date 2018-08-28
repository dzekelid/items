{
  "info": {
    "name": "Plentymarkets Update an item set configuration",
    "_postman_id": "c4a3014c-7030-4178-b849-8531a6f213ef",
    "description": "Update an item set configuration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "095bad08-4aaf-4a3c-96db-4d9db6dab58b",
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
              "id": "1f31cfff-bc99-43b5-8e76-9318424f39c5"
            }
          ]
        },
        {
          "id": "ffc5df9c-cabd-477f-95a9-be0a8577ad97",
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
              "id": "eb2dd68e-ac3b-40b1-856d-b26672caf8a0"
            }
          ]
        },
        {
          "id": "6dc1de58-f328-4f92-8492-8a8073c0cb12",
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
              "id": "cd107bfc-09e1-4f9d-ab35-85386e479570"
            }
          ]
        }
      ]
    },
    {
      "name": "Revenue",
      "item": [
        {
          "id": "00f556ee-ae57-4947-b794-157af0a0962c",
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
              "id": "1c4d8a57-df20-4742-92f3-08760ea4f04d"
            }
          ]
        },
        {
          "id": "76f249d7-aa4d-4f13-89d2-2384a09bb61f",
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
              "id": "606f1899-ee1f-4e19-879b-936aa4ea1fb4"
            }
          ]
        }
      ]
    },
    {
      "name": "Debtor",
      "item": [
        {
          "id": "3dff8193-acb5-4d11-8932-2486ce4499fd",
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
              "id": "ab8fa62d-1caf-4982-ab5e-e264490991c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "c9bb9383-ac10-4261-a2e2-3e5b05aaf55b",
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
              "id": "74981035-3e69-48cf-a761-6925a03d481f"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "7ed4f980-2c57-4da3-9fd7-9aba89065b69",
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
              "id": "e9b0bdc6-6d4f-4418-b910-d4891aacf8c7"
            }
          ]
        },
        {
          "id": "d3af064c-346d-43fc-b340-2c374fa0819d",
          "name": "putRestItemSetsSetConfig",
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
            "description": "Update an item set configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0493adf9-0695-4938-a022-b8becd316673"
            }
          ]
        }
      ]
    }
  ]
}