swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 1
info:
  title: Content API for Shopping
  description: manages-product-items-inventory-and-merchant-center-accounts-for-google-shopping-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{merchantId}/orders/{orderId}/cancelLineItem:
    post:
      summary: Cancel Order Line Item
      description: Cancels a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.cancellineitem
      x-api-path-slug: merchantidordersorderidcancellineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
      - Line
      - Item
  /{merchantId}/orders/{orderId}/returnLineItem:
    post:
      summary: Return Line Item
      description: Returns a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.returnlineitem
      x-api-path-slug: merchantidordersorderidreturnlineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Return
      - Line
      - Item
  /{merchantId}/orders/{orderId}/shipLineItems:
    post:
      summary: Ship Line Item
      description: Marks line item(s) as shipped. This method can only be called for
        non-multi-client accounts.
      operationId: content.orders.shiplineitems
      x-api-path-slug: merchantidordersorderidshiplineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Ship
      - Line
      - Item