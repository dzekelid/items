---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List basket items
  description: Lists all items in the shopping cart for the current customer session.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/basket/items:
    get:
      summary: List basket items
      description: Lists all items in the shopping cart for the current customer session.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitems-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Basket
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