{
  "info": {
    "name": "Kentico Cloud Delete a content item by codename",
    "_postman_id": "e508e7c3-e4bb-4fb7-b5c6-2ab379facb47",
    "description": "Delete a content item specified by its codename.\n\nNote that deleting a content item deletes all of its language variants as well.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "9c27e389-f65b-4731-a250-c12006b86f3a",
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
              "id": "e1a5a3f8-7ea6-46e8-acb4-1ddaf1cd4a46"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "2d76aff5-f2aa-40f9-bce4-c5068bdaef37",
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
              "id": "ea6f1ecb-38f9-4b32-9a44-104d09a3c8dc"
            }
          ]
        },
        {
          "id": "62466b6e-3dda-4e08-9c67-ae49ccfffbe3",
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
              "id": "5277c87d-e7a8-450d-b05e-f31a2084f30b"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "1afb3ecd-2b28-4834-9bfa-81d177e67d26",
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
              "id": "5a0fc145-4f3b-4e80-a208-e217713e8cd1"
            }
          ]
        },
        {
          "id": "7bf5d46f-06b2-441e-b9f6-8723f16f743b",
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
              "id": "a4808e2a-0fd0-47ba-bd29-37ddc479428a"
            }
          ]
        },
        {
          "id": "9113df10-733d-4faf-8550-fb5712e78c94",
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
              "id": "3c1c2f53-9cd0-4942-be46-74292a90d044"
            }
          ]
        },
        {
          "id": "06964d8e-9849-4cd2-8078-d011b54a4e1f",
          "name": "ItemsCodenameOnRoastsDelete",
          "request": {
            "url": "http://deliver.kenticocloud.com/items/codename/on_roasts",
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
            "description": "Delete a content item specified by its codename.\n\nNote that deleting a content item deletes all of its language variants as well."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fbbf158-d6a2-4e0f-9a20-86e873ec4251"
            }
          ]
        }
      ]
    },
    {
      "name": "Filtering",
      "item": [
        {
          "id": "6c669e21-aacd-4b8f-924e-b570164023fa",
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
              "id": "c8172b1e-4cf2-4b26-b9fe-cd055d5b9d86"
            }
          ]
        }
      ]
    }
  ]
}