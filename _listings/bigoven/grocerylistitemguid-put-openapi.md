---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Update a grocery item by GUID
  description: Update a grocery item by guid.
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /grocerylist/item:
    post:
      summary: Add a single line item to the grocery list
      description: Add a single line item to the grocery list.
      operationId: GroceryList_Post
      x-api-path-slug: grocerylistitem-post
      parameters:
      - in: body
        name: newItem
        description: name, quantity, unit, notes, department
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
  /grocerylist/item/{guid}:
    delete:
      summary: /grocerylist/item/{guid}  DELETE will delete this item assuming you
        own it.
      description: /grocerylist/item/{guid}  delete will delete this item assuming
        you own it..
      operationId: GroceryList_DeleteItemByGuid
      x-api-path-slug: grocerylistitemguid-delete
      parameters:
      - in: path
        name: guid
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
    put:
      summary: Update a grocery item by GUID
      description: Update a grocery item by guid.
      operationId: GroceryList_GroceryListItemGuid
      x-api-path-slug: grocerylistitemguid-put
      parameters:
      - in: path
        name: guid
      - in: body
        name: req
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
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