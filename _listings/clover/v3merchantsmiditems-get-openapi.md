---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all inventory items
  version: 1.0.0
  description: Get all inventory items.
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