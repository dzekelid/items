{
  "info": {
    "name": "Kentico Cloud Update a content item by ID",
    "_postman_id": "01cff5b6-322c-44d3-a6bb-e0057f93f3c7",
    "description": "Update an existing content item specified by its internal ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "00635b5e-c473-4b6a-9aef-edcce5befbcb",
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
              "id": "e0d18341-f7c9-4f55-ac75-e507fccaa755"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "ceca4fe0-5966-491c-ba79-120021b25976",
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
              "id": "e58bc8b3-0761-4d78-8e8c-2426a7627eec"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "bdc06f85-64ce-46d8-bc3c-c03d1e0bdfe6",
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
              "id": "fc51a8eb-6815-4ddf-9082-dae8c34036fa"
            }
          ]
        }
      ]
    }
  ]
}