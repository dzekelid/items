swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/carts/active/line-items:
    delete:
      summary: Delete Shoppers Me Carts Active Line Items
      description: Delete shoppers me carts active line items.
      operationId: deleteV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-delete
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    get:
      summary: Get Shoppers Me Carts Active Line Items
      description: Get shoppers me carts active line items.
      operationId: getV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    post:
      summary: Post Shoppers Me Carts Active Line Items
      description: Post shoppers me carts active line items.
      operationId: postV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
  /v1/shoppers/me/carts/active/line-items/{id}:
    delete:
      summary: Delete Shoppers Me Carts Active Line Items
      description: Delete shoppers me carts active line items.
      operationId: deleteV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    get:
      summary: Get Shoppers Me Carts Active Line Items
      description: Get shoppers me carts active line items.
      operationId: getV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    post:
      summary: Post Shoppers Me Carts Active Line Items
      description: Post shoppers me carts active line items.
      operationId: postV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
  /v1/shoppers/me/orders/{id}/line-items:
    get:
      summary: Get Shoppers Me Orders Line Items
      description: Get shoppers me orders line items.
      operationId: getV1ShoppersMeOrdersLineItems
      x-api-path-slug: v1shoppersmeordersidlineitems-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Line
      - Items
  /v1/shoppers/me/orders/{id}/line-items/{lineItemId}:
    get:
      summary: Get Shoppers Me Orders Line Items Lineitemid
      description: Get shoppers me orders line items lineitemid.
      operationId: getV1ShoppersMeOrdersLineItemsLineitem
      x-api-path-slug: v1shoppersmeordersidlineitemslineitemid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lineItemId
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Line
      - Items
      - Lineitemid