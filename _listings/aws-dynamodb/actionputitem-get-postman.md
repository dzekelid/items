{
  "info": {
    "name": "Amazon DynamoDB API Put Item",
    "_postman_id": "7a042c96-bb6d-4b95-902e-79d4a6073c88",
    "description": "Creates a new item, or replaces an old item with a new item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "e1d50807-6145-41c1-8190-25b98b9adc1e",
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
              "id": "d5004a4a-a5ba-49a2-863c-ca3c0293c972"
            }
          ]
        },
        {
          "id": "6c552bda-07e2-4081-bc65-fac22f354244",
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
              "id": "08ec40c7-a1c6-4c25-b518-b44263da84cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "9b7d343a-bce1-47f2-b3a8-375a2db03178",
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
              "id": "eebb153f-b8ea-46a2-b1ab-4bf564b99ddd"
            }
          ]
        },
        {
          "id": "436e1217-92ed-4c8b-b7b8-98044dff3a2b",
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
              "id": "943fa373-2c1f-49de-a8cb-57853bfe747e"
            }
          ]
        },
        {
          "id": "46dd27e0-657b-40eb-bd3a-6f5797bf6f93",
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
              "id": "289082bc-b56d-4552-986d-bdd543f5f10a"
            }
          ]
        },
        {
          "id": "768625c3-245a-4aef-8a84-a10646543248",
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
              "id": "fcf2298f-77f6-4fff-90bb-536aade6e9c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "0bb58e28-0535-42ef-ad67-321302ab16b5",
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
              "id": "fb5e8f45-651e-4b52-b5fc-f01c559a2083"
            }
          ]
        },
        {
          "id": "7888cfb1-e94b-40eb-822c-763b1a67718a",
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
              "id": "d6bd5407-60ad-4db8-81b6-2b7f8416208c"
            }
          ]
        },
        {
          "id": "2299330c-3f76-4b4e-80e0-84c04679e189",
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
              "id": "12f7209d-0771-44fa-9b15-c3db3db14a0f"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "f3770c50-ae38-46d4-8b9f-14c841228d47",
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
              "id": "4bff60e0-07d1-47cc-8df4-a0f7465372ef"
            }
          ]
        }
      ]
    }
  ]
}