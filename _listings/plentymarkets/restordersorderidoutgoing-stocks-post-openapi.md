---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Book out order items
  description: Books out the order items of an order. The ID of the order must be
    specified and a booking date can be specified. The current date and time will
    be used if no date is specified.
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
  /rest/items/item_shipping_profiles:
    get:
      summary: List all shipping profiles of all items
      description: |-
        Lists all shipping profiles of all items. Results can be filtered by the timestamp of the link between items and shipping profiles (eq, lt, lte, gt, gte, between).
        <ul>
        <li>eq = Equal to</li>
        <li>gte = Greater than or equal to</li>
        <li>gt = Greater than</li>
        <li>lte = Less than or equal to</li>
        <li>lt = Less than</li>
        <li>between = Date range</li>
        </ul>
        Example: updated=gt:2018-04-16 16:00:00 returns all items with shipping profiles that were activated after 4pm on the 16th of April 2018.
      operationId: getRestItemsItemShippingProfiles
      x-api-path-slug: restitemsitem-shipping-profiles-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Shipping
      - Profiles
      - Of
      - ""
      - Items
  /rest/orders/{orderId}/outgoing_stocks:
    post:
      summary: Book out order items
      description: Books out the order items of an order. The ID of the order must
        be specified and a booking date can be specified. The current date and time
        will be used if no date is specified.
      operationId: postRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-post
      parameters:
      - in: query
        name: date
        description: The date that is saved as booking date for the outgoing stock
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Out
      - Order
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