{
  "info": {
    "name": "Plentymarkets Delete an item set component",
    "_postman_id": "66fa560a-620e-474f-a908-eee494697c4a",
    "description": "Deletes an item set component. The item set component ID of the item set component must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "d539ed23-dd3c-444c-b719-f2961433c25c",
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
              "id": "4c4ca423-ed52-4696-845b-cedf72cfc73a"
            }
          ]
        },
        {
          "id": "c6069c47-5137-4875-b1a0-12afa0cf17b3",
          "name": "getRestItemsVariationsVariationVariationBundles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_bundles"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
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
            "description": "List all components of a bundle. The ID of the item and the ID of the variation to which bundle components were added must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92a31ecd-17b0-4673-b74f-6fe6a7c79874"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "ed53a4ea-a293-4a1e-8041-97427fe5e2fe",
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
              "id": "dc601118-1c83-4cdd-8549-7770ec0b21af"
            }
          ]
        },
        {
          "id": "b53a2c8d-e45e-4fc6-8d28-6f111e86674d",
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
              "id": "a67d1b9a-36c1-4636-a8fd-ef2fd3b6eedd"
            }
          ]
        },
        {
          "id": "ebc14276-d9ac-4cd3-8f03-1426586ec4c9",
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
              "id": "470f4486-d546-471d-a14b-4ebcf408e186"
            }
          ]
        },
        {
          "id": "3ef09af6-28eb-4e9f-b35d-1c18c6ace4fd",
          "name": "getRestItemSetsSetComponents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/components/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get an item set component."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "362f3dd3-5422-4862-8336-d7124d0188c1"
            }
          ]
        },
        {
          "id": "f0a6e9b6-dbf0-43b9-9487-ed448809fe2f",
          "name": "putRestItemSetsSetComponents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/components/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Update an item set component."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4eed2bba-4ef0-4228-9138-77f964879195"
            }
          ]
        },
        {
          "id": "8e858f72-1a51-40c5-a348-2366b2a2f9ef",
          "name": "deleteRestItemSetsSetComponents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/components/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Deletes an item set component. The item set component ID of the item set component must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59d201fe-7b7b-4121-92f1-8f50f02f78fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "32f34af0-9452-44b3-ac07-85f1a8ad7f29",
          "name": "deleteRestItemsVariationsVariationVariationBundlesBundle",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_bundles/:bundleId"
              ],
              "variable": [
                {
                  "id": "bundleId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
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
            "description": "Removes a component from a bundle. The bundle ID must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebb3386f-2451-49df-8241-3c6b4a9fcd0b"
            }
          ]
        }
      ]
    }
  ]
}