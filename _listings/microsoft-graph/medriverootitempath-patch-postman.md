{
  "info": {
    "name": "Microsoft Graph API Update Drive Item Properties",
    "_postman_id": "45395e13-e67d-452a-8591-61d37502cb14",
    "description": "Update DriveItem properties Update the metadata for a DriveItem by ID or path.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "drive",
      "item": [
        {
          "id": "3da96ca4-f982-4654-a0bb-374cb0ab1e5e",
          "name": "UpdateDriveItemProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/drive/root:/:item-path"
              ],
              "variable": [
                {
                  "id": "item-path",
                  "value": "item-path",
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
              "id": "013d0ad1-44d1-4265-bd2e-756e83159b78"
            }
          ]
        }
      ]
    }
  ]
}