---
swagger: "2.0"
x-collection-name: AWS DynamoDB
x-complete: 0
info:
  title: Amazon DynamoDB API Put Item
  version: 1.0.0
  description: Creates a new item, or replaces an old item with a new item.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteItem:
    get:
      summary: Delete Item
      description: Deletes a single item in a table by primary key.
      operationId: deleteItem
      x-api-path-slug: actiondeleteitem-get
      parameters:
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          DeleteItem to      succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Key
        description: A map of attribute names to AttributeValue objects, representing
          the primary key of      the item to delete
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared before they      were deleted
        type: string
      - in: query
        name: TableName
        description: The name of the table from which to delete the item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=GetItem:
    get:
      summary: Get Item
      description: |-
        The GetItem operation returns a set of attributes for the item with the given primary
                  key.
      operationId: getItem
      x-api-path-slug: actiongetitem-get
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'Determines the read consistency model:  If set to true, then
          the operation uses strongly consistent reads; otherwise, the operation uses
          eventually consistent reads'
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: Key
        description: A map of attribute names to AttributeValue objects, representing
          the primary key of      the item to retrieve
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the table
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=PutItem:
    get:
      summary: Put Item
      description: Creates a new item, or replaces an old item with a new item.
      operationId: putItem
      x-api-path-slug: actionputitem-get
      parameters:
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          PutItem operation to      succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Item
        description: A map of attribute name/value pairs, one for each attribute
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared before they      were updated with the PutItem request
        type: string
      - in: query
        name: TableName
        description: The name of the table to contain the item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=UpdateItem:
    get:
      summary: Update Item
      description: Edits an existing item's attributes, or adds a new item to the
        table if it does not already exist.
      operationId: updateItem
      x-api-path-slug: actionupdateitem-get
      parameters:
      - in: query
        name: AttributeUpdates
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          update to succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Key
        description: The primary key of the item to be updated
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared either before      or after they were updated
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the item to update
        type: string
      - in: query
        name: UpdateExpression
        description: An expression that defines one or more attributes to be updated,
          the action to be performed on them, and new value(s) for them
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=BatchGetItem:
    get:
      summary: Batch Get Item
      description: |-
        The BatchGetItem operation returns the attributes of one or more items from one or
              more tables.
      operationId: batchGetItem
      x-api-path-slug: actionbatchgetitem-get
      parameters:
      - in: query
        name: RequestItems
        description: A map of one or more table names and, for each table, a map that
          describes one or more items to retrieve from that table
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Batch Items
  /?Action=BatchWriteItem:
    get:
      summary: Batch Write Item
      description: The BatchWriteItem operation puts or deletes multiple items in
        one or more tables.
      operationId: batchWriteItem
      x-api-path-slug: actionbatchwriteitem-get
      parameters:
      - in: query
        name: RequestItems
        description: A map of one or more table names and, for each table, a list
          of operations to be performed        (DeleteRequest or PutRequest)
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Batch Items
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---