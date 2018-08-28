{
  "info": {
    "name": "Microsoft Graph API Update Drive Item Properties",
    "_postman_id": "05ec64c3-8148-4ff5-99ba-649d867ca3c7",
    "description": "Update DriveItem properties Update the metadata for a DriveItem by ID or path.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "drive",
      "item": [
        {
          "id": "6a479770-975f-4ca0-981b-72476cd3bc91",
          "name": "UpdateDriveItemProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "drives/:drive-id/items/:item-id"
              ],
              "variable": [
                {
                  "id": "drive-id",
                  "value": "drive-id",
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
              "id": "dde9645e-56b0-4708-8d86-2a8dab5503be"
            }
          ]
        }
      ]
    }
  ]
}