---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Update existing inventory items.
  version: 1.0.0
  description: This API is to going to update only the changes present in the payload.
    Not going to replace the existing inventory items. Use the POST HTTP method to
    create inventory items.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/items:
    get:
      summary: Get all inventory items
      description: Get all inventory items.
      operationId: GetItems
      x-api-path-slug: v3merchantsmiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, sku, modifiedTime, deleted, hidden,
          price, alternateName, itemCode, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    post:
      summary: Create an inventory item
      description: Create an inventory item.
      operationId: CreateItem
      x-api-path-slug: v3merchantsmiditems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    delete:
      summary: Bulk delete inventory items
      description: Bulk delete inventory items.
      operationId: BulkDeleteItems
      x-api-path-slug: v3merchantsmiditems-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
  /v3/merchants/{mId}/items/{itemId}:
    get:
      summary: Get a single inventory item
      description: Get a single inventory item.
      operationId: GetItem
      x-api-path-slug: v3merchantsmiditemsitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    post:
      summary: Update an existing inventory item
      description: Update an existing inventory item.
      operationId: UpdateItem
      x-api-path-slug: v3merchantsmiditemsitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    delete:
      summary: Delete an inventory item
      description: Delete an inventory item.
      operationId: DeleteItem
      x-api-path-slug: v3merchantsmiditemsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
  /v3/merchants/{mId}/bulk_items:
    post:
      summary: Create multiple inventory items.
      description: This API is to create multiple inventory items.  Use the PATCH
        HTTP method to update existing inventory items.
      operationId: BulkCreateInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
      - Items
    put:
      summary: Update existing inventory items.
      description: This API is to going to update only the changes present in the
        payload. Not going to replace the existing inventory items. Use the POST HTTP
        method to create inventory items.
      operationId: BulkPatchInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
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