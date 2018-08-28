{
  "info": {
    "name": "Kentico Cloud Delete a content item by ID",
    "_postman_id": "959425b4-f141-4f86-a2a4-d93bc874a1d8",
    "description": "Delete a content item specified by its internal ID. Note that deleting a content item deletes all of its language variants as well.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "648aba0d-3f8c-4e71-9718-952533b4fb4d",
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
              "id": "e8a170d3-e008-43ec-835e-b1a539e49e49"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "107bae05-820d-4b91-a0d9-1c02ffc0ff4e",
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
              "id": "24ab9266-912a-4747-a72a-441821114489"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "e5857ad8-648c-42d1-82b5-a15d27ab42d8",
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
              "id": "25865253-115d-4d93-a083-8c3e170a10a1"
            }
          ]
        },
        {
          "id": "1431aea1-c48c-4c4b-b6c7-658378757734",
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
              "id": "5eef4239-26b3-4769-95c3-ccef1d632276"
            }
          ]
        }
      ]
    }
  ]
}