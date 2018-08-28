{
  "info": {
    "name": "Microsoft Graph API Update Drive Item Properties",
    "_postman_id": "3abd6f64-516a-4b65-8bb0-5cd9395e46b5",
    "description": "Update DriveItem properties Update the metadata for a DriveItem by ID or path.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "drive",
      "item": [
        {
          "id": "f4ca04e4-f29c-4cc2-9044-f9730b2550bb",
          "name": "UpdateDriveItemProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:group-id/drive/items/:item-id"
              ],
              "variable": [
                {
                  "id": "group-id",
                  "value": "group-id",
                  "type": "string"
                },
                {
                  "id": "item-id",
                  "value": "item-id",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "if-match",
                "value": "if-match",
                "description": "If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a 412 Precondition Failed response is returned",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update DriveItem properties Update the metadata for a DriveItem by ID or path"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "dc0b5538-0759-442a-b8f8-de6acdaa977a"
            }
          ]
        }
      ]
    }
  ]
}