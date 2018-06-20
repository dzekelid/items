{
  "info": {
    "name": "Amazon DynamoDB API Update Item",
    "_postman_id": "5a1a09f1-cf07-4819-b2ae-2c305f9f810e",
    "description": "Edits an existing item's attributes, or adds a new item to the table if it does not already exist.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "1a9a38ba-6839-498f-a6c5-48846f465170",
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
              "id": "0876025c-acb1-4151-ba9b-a01eb253d5f8"
            }
          ]
        },
        {
          "id": "31d2111e-d436-4a6f-8156-fb33348eafdb",
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
              "id": "cb8ced2c-4e9e-410a-bbd5-c25ef342c3e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "7ce1c001-7ad1-4b95-bbbb-1a0f20d7c632",
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
              "id": "2904aa06-2c94-4a88-846a-8b0440dc9976"
            }
          ]
        },
        {
          "id": "62463399-f7a9-45af-afae-9a6eef54e5e0",
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
              "id": "a659321c-2d44-4c3f-a45f-6b37637e5f7f"
            }
          ]
        },
        {
          "id": "5ac7e577-0a66-40eb-8b5f-752e91a0ef4b",
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
              "id": "5f24ac07-9143-4f1f-9bc1-9359bbd065fc"
            }
          ]
        },
        {
          "id": "c2f42e51-56d7-4e01-a544-35f566dd05b0",
          "name": "listTables",
          "request": {
            "url": "http://example.com/api/?Action=ListTables?ExclusiveStartTableName=ExclusiveStartTableName&Limit=Limit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of table names associated with the current account and endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "258075e3-8371-411e-9640-43342afc406e"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "97a03c81-1630-48b1-bf39-6d5cec455b44",
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
              "id": "ad21ab09-7b6e-438a-9c15-da82f640ae90"
            }
          ]
        },
        {
          "id": "b695bffa-0227-42f4-b7f1-70c543ae7f59",
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
              "id": "92bda381-ab48-4d45-b133-248015bb7506"
            }
          ]
        },
        {
          "id": "1ae0cd8f-b805-4f9a-9b16-457ea7eed12a",
          "name": "putItem",
          "request": {
            "url": "http://example.com/api/?Action=PutItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Item=Item&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new item, or replaces an old item with a new item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7304e7f-9ad7-41da-8dea-d2f5155c35ca"
            }
          ]
        },
        {
          "id": "6c43101c-cd05-4e81-bcae-fe322a576cf9",
          "name": "updateItem",
          "request": {
            "url": "http://example.com/api/?Action=UpdateItem?AttributeUpdates=AttributeUpdates&ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Key=Key&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName&UpdateExpression=UpdateExpression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Edits an existing item's attributes, or adds a new item to the table if it does not already exist."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a19062b-95cd-49ec-928a-adcfcdcf5e1d"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "cb466a64-02e5-4dd1-9e55-fad0ac97874c",
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
              "id": "95244556-eea1-46cc-8501-21062f1575ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Query",
      "item": [
        {
          "id": "1ffd36fc-39ef-4ca1-ab12-3a0c360fbb0c",
          "name": "query",
          "request": {
            "url": "http://example.com/api/?Action=Query?AttributesToGet=AttributesToGet&ConditionalOperator=ConditionalOperator&ConsistentRead=ConsistentRead&ExclusiveStartKey=ExclusiveStartKey&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&FilterExpression=FilterExpression&IndexName=IndexName&KeyConditionExpression=KeyConditionExpression&KeyConditions=KeyConditions&Limit=Limit&ProjectionExpression=ProjectionExpression&QueryFilter=QueryFilter&ReturnConsumedCapacity=ReturnConsumedCapacity&ScanIndexForward=ScanIndexForward&Select=Select&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Query operation uses the primary key of a table or a secondary index\n            to directly access items from that table or index."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "968ea9c5-c36b-436e-8c8d-ee03807c1699"
            }
          ]
        }
      ]
    },
    {
      "name": "Scan",
      "item": [
        {
          "id": "8660ae01-c9ef-4f07-9b7b-ba2b6358eddc",
          "name": "scan",
          "request": {
            "url": "http://example.com/api/?Action=Scan?AttributesToGet=AttributesToGet&ConditionalOperator=ConditionalOperator&ConsistentRead=ConsistentRead&ExclusiveStartKey=ExclusiveStartKey&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&FilterExpression=FilterExpression&IndexName=IndexName&Limit=Limit&ProjectionExpression=ProjectionExpression&ReturnConsumedCapacity=ReturnConsumedCapacity&ScanFilter=ScanFilter&Segment=Segment&Select=Select&TableName=TableName&TotalSegments=TotalSegments",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Scan operation returns one or more items and item attributes by accessing every\n      item in a table or a secondary index."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa5cb74f-9806-4ff4-87b1-95f6c862280c"
            }
          ]
        }
      ]
    }
  ]
}