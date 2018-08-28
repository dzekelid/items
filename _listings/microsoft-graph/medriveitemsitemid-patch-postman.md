{
  "info": {
    "name": "Microsoft Graph API Update Drive Item Properties",
    "_postman_id": "2f59b9e5-93b1-4913-a235-fc5877f8eaf0",
    "description": "Update DriveItem properties Update the metadata for a DriveItem by ID or path.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "drive",
      "item": [
        {
          "id": "460ae445-8786-4788-a03d-494d66d84e17",
          "name": "UpdateDriveItemProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/drive/items/:item-id"
              ],
              "variable": [
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
              "id": "1dd97a34-39fe-4010-bc33-4e41793d178e"
            }
          ]
        }
      ]
    }
  ]
}