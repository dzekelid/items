{
  "info": {
    "name": "Amazon DynamoDB API Batch Get Item",
    "_postman_id": "3c417dd0-aa25-4b5d-a1a2-dea351b9f8e0",
    "description": "The BatchGetItem operation returns the attributes of one or more items from one or\n      more tables.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "d51d1f46-3318-4fb8-9ef7-10538614bdd8",
          "name": "batchGetItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchGetItem operation returns the attributes of one or more items from one or\n      more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53b0ad45-10c6-4963-8d24-07380017cc54"
            }
          ]
        }
      ]
    }
  ]
}