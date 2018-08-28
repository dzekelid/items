swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4554953422/refunds/calculate.json:
    post:
      summary: Calculate a refund for a line item and shipping
      description: Calculate a refund for a line item and shipping.
      operationId: postAdminOrders4554953422RefundsCalculate.json
      x-api-path-slug: adminorders4554953422refundscalculate-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Calculate
      - Refunda
      - Line
      - Item
      - Shipping