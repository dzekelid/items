{
  "info": {
    "name": "Amazon DynamoDB API Batch Write Item",
    "_postman_id": "8a64a5b4-512e-4d57-ab73-4d5dacbe15de",
    "description": "The BatchWriteItem operation puts or deletes multiple items in one or more tables.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "15c4e459-a4a1-4ab7-9e0e-4b7e8444199d",
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
              "id": "2acd6170-e7b7-470c-b6c1-a14fa99f6921"
            }
          ]
        },
        {
          "id": "5cf2bd8a-153e-478e-bc1c-26f545836c7d",
          "name": "batchWriteItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchWriteItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchWriteItem operation puts or deletes multiple items in one or more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b03a2fb8-1774-40d8-9579-b8ac112950e7"
            }
          ]
        }
      ]
    }
  ]
}