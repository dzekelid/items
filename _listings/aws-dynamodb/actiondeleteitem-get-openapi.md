---
swagger: "2.0"
x-collection-name: AWS DynamoDB
x-complete: 0
info:
  title: Amazon DynamoDB API Delete Item
  version: 1.0.0
  description: Deletes a single item in a table by primary key.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
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