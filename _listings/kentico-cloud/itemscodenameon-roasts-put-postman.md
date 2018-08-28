{
  "info": {
    "name": "Kentico Cloud Update a content item by codename",
    "_postman_id": "22e86e4a-f741-460d-8168-22630281e50a",
    "description": "Update an existing content item specified by its codename.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "4c984a03-7ebb-4756-8d5e-17295bc79a80",
          "name": "975bf280Fd91488c994c2f04416e5ee3ItemsGet8",
          "request": {
            "url": "http://deliver.kenticocloud.com/975bf280-fd91-488c-994c-2f04416e5ee3/items?order=%7B%7D&system.type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Filter the content items by content type by including the `order` query parameter and a content element codename."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c112fd4-a210-4eb5-9407-412ae4d46704"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "807dfec7-fe05-4b21-b1b7-3a8f79c3fe67",
          "name": "Items3120ec15A4a247ec8ccdC85ac8ac5ba5Get",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve metadata information about a content item specified by its internal ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b0225e3-57fb-4b1a-bbb9-dbad411bff26"
            }
          ]
        },
        {
          "id": "f24fd1ba-a5e7-4870-82bf-5202e0fc00c0",
          "name": "ItemsCodenameOnRoastsGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/codename/on_roasts",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve metadata information about a content item specified by its codename."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f06a0782-7e8a-40f6-9d83-7b9ae0890f8f"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "e8f64eb6-1b97-4aaa-b6bf-8ca97a2026bd",
          "name": "Items3120ec15A4a247ec8ccdC85ac8ac5ba5Put",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing content item specified by its internal ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0092aa24-ec91-4953-a433-b3d041009c82"
            }
          ]
        },
        {
          "id": "0b7116b0-074f-4ad6-b317-fda5dd7ffac6",
          "name": "Items3120ec15A4a247ec8ccdC85ac8ac5ba5Delete2",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5",
            "method": "DELETE",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete a content item specified by its internal ID. Note that deleting a content item deletes all of its language variants as well."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4ea14c5-cbe3-4d75-b363-15ac943092ff"
            }
          ]
        },
        {
          "id": "060b913b-4c04-43c5-9804-8e4e4b1edf07",
          "name": "ItemsCodenameOnRoastsPut",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/codename/on_roasts",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing content item specified by its codename."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b47ea192-751a-48a8-8c29-5a0b78fd0bbe"
            }
          ]
        }
      ]
    },
    {
      "name": "Filtering",
      "item": [
        {
          "id": "4f3acd78-eaa5-4b04-aaae-7c526a5eea48",
          "name": "143728440a5d434a8423605b8a631623ItemsGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/14372844-0a5d-434a-8423-605b8a631623/items?elements.publish_until[gt]=%7B%7D&system.type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Filter content items directly in the API call using the `element.element_codename` query parameter and *publish from* and *publish until* elements.\n\nSee <https://developer.kenticocloud.com/docs/scheduling-content-unpublishing#section-filtering-by-date-with-the-delivery-api> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bfe7e02-0157-415e-b0b1-71dd1c5cdd67"
            }
          ]
        }
      ]
    }
  ]
}