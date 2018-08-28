{
  "info": {
    "name": "Amazon DynamoDB API Get Item",
    "_postman_id": "3dd65168-bc20-4c5a-9afd-8402cf27b8e1",
    "description": "The GetItem operation returns a set of attributes for the item with the given primary\n          key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "f2cba09c-0d92-4585-ac0d-39773e15cfae",
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
              "id": "7f9f25e0-1a48-4313-9405-b46e0cc5a8fa"
            }
          ]
        },
        {
          "id": "11058efa-bd9a-4a16-b0ee-584b0f21e9e5",
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
              "id": "f98b8f37-9222-4226-a090-0eb072cf9336"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "2c803b84-3683-41c6-81c1-1d01df951081",
          "name": "createTable",
          "request": {
            "url": "http://example.com/api/?Action=CreateTable?AttributeDefinitions=AttributeDefinitions&GlobalSecondaryIndexes=GlobalSecondaryIndexes&KeySchema=KeySchema&LocalSecondaryIndexes=LocalSecondaryIndexes&ProvisionedThroughput=ProvisionedThroughput&StreamSpecification=StreamSpecification&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The CreateTable operation adds a new table to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "660b7fe3-4262-4947-a348-3f1343a0a326"
            }
          ]
        },
        {
          "id": "8ca678b1-0d1c-4272-b8b7-2144641bffc5",
          "name": "deleteTable",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteTable operation deletes a table and all of its items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e86306a-3489-420c-91d9-9e89f3f610d9"
            }
          ]
        },
        {
          "id": "69415d89-af97-47a9-9134-88ecf452ea79",
          "name": "describeTable",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the table, including the current status of the table, when it was created, the primary key schema, and any indexes on the table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "269c2152-c0f3-4460-bebc-42cc0125e98a"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "75fd34e2-4fcd-4964-8c1b-c93c3487da79",
          "name": "deleteItem",
          "request": {
            "url": "http://example.com/api/?Action=DeleteItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Key=Key&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a single item in a table by primary key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f8f8577-450f-494c-ae0d-0483260b5d27"
            }
          ]
        },
        {
          "id": "51f1d18f-b291-4d01-ae12-c14d28c26461",
          "name": "getItem",
          "request": {
            "url": "http://example.com/api/?Action=GetItem?AttributesToGet=AttributesToGet&ConsistentRead=ConsistentRead&ExpressionAttributeNames=ExpressionAttributeNames&Key=Key&ProjectionExpression=ProjectionExpression&ReturnConsumedCapacity=ReturnConsumedCapacity&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The GetItem operation returns a set of attributes for the item with the given primary\n          key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78a832dd-27a4-4750-8693-ad7b87d152c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "7ba8449e-9fad-4e81-819b-755c889dea17",
          "name": "describeLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLimits?AccountMaxReadCapacityUnits=AccountMaxReadCapacityUnits&AccountMaxWriteCapacityUnits=AccountMaxWriteCapacityUnits&TableMaxReadCapacityUnits=TableMaxReadCapacityUnits&TableMaxWriteCapacityUnits=TableMaxWriteCapacityUnits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current provisioned-capacity limits for your AWS account in a region, both for the region as a whole and for any one DynamoDB table that you create there."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5fcb442-36c9-44cc-9c9a-3d40f78a9313"
            }
          ]
        }
      ]
    }
  ]
}