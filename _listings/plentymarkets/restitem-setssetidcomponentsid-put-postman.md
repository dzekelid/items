{
  "info": {
    "name": "Plentymarkets Update an item set component",
    "_postman_id": "99ae0cc4-a537-4778-aec6-eed7e8db759a",
    "description": "Update an item set component.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "fa038845-dd45-4d98-9720-e96b9021a6ba",
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
              "id": "cbd3e8fb-e9e6-454d-936f-68fd0390714d"
            }
          ]
        },
        {
          "id": "723aca5e-2af7-499c-8364-96a66936a1ae",
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
              "id": "ce634181-eafb-4dd1-af36-ed849ec9c259"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "6eba4628-8348-4da7-b5af-c084d90366f5",
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
              "id": "cd9f00d5-6327-47c6-a2ea-b5b1566927d0"
            }
          ]
        },
        {
          "id": "f6faf5b1-cecf-4799-98d6-4a5c68e614cb",
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
              "id": "1572fe64-33c6-4612-9536-c850428b3a24"
            }
          ]
        },
        {
          "id": "4d9626d2-2d97-4008-8c89-967a8bc65bf4",
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
              "id": "35fa413f-2977-4541-a0d4-583d5539b5be"
            }
          ]
        },
        {
          "id": "c5529411-f7aa-40d2-9282-0c39e4b0d71b",
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
              "id": "d96d851e-4c65-4745-b246-d077bffad18b"
            }
          ]
        },
        {
          "id": "e9bab92c-13f3-4cdc-a23b-6c32de8fb28e",
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
              "id": "f45fe8ec-44d3-41d1-9b40-3272d55578a4"
            }
          ]
        },
        {
          "id": "8c6d6c1f-199c-41dc-8ab8-b41c972d8f48",
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
              "id": "12d8aeee-9f76-4fb9-91f9-3ccd30246542"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "9af5f638-c384-46fa-aec5-58dda4945cc0",
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
              "id": "010d3241-330d-426a-b582-2f8ffe3959b3"
            }
          ]
        }
      ]
    }
  ]
}