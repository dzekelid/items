---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Put Wishlist Items
  description: Put wishlist items.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/{cartId}/items/{itemId}:
    put:
      summary: Put Cart Items
      description: Put cart items.
      operationId: putCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: query
        name: quantity
        description: quantity
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
    delete:
      summary: Delete Cart Items
      description: Delete cart items.
      operationId: deleteCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
  /wishlist/items/{itemId}:
    put:
      summary: Put Wishlist Items
      description: Put wishlist items.
      operationId: putWishlistItemsItem
      x-api-path-slug: wishlistitemsitemid-put
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: quantity
        description: quantity
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
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