---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Items:
    get:
      summary: Get Items
      description: Get items.
      operationId: getItems
      x-api-path-slug: items-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
    post:
      summary: Post Items
      description: Post items.
      operationId: postItems
      x-api-path-slug: items-post
      parameters:
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
    put:
      summary: Put Items
      description: Put items.
      operationId: putItems
      x-api-path-slug: items-put
      parameters:
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
    x-related-model:
      summary: X-related-model Items
      description: X-related-model items.
      operationId: x-related-modelItems
      x-api-path-slug: items-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Items
  /Items/{ItemID}:
    delete:
      summary: Delete Items
      description: Delete items item.
      operationId: deleteItemsItem
      x-api-path-slug: itemsitemid-delete
      parameters:
      - in: path
        name: ItemID
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    get:
      summary: Get Items
      description: Get items item.
      operationId: getItemsItem
      x-api-path-slug: itemsitemid-get
      parameters:
      - in: path
        name: ItemID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    post:
      summary: Post Items
      description: Post items item.
      operationId: postItemsItem
      x-api-path-slug: itemsitemid-post
      parameters:
      - in: path
        name: ItemID
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    x-related-model:
      summary: X-related-model Items
      description: X-related-model items item.
      operationId: x-related-modelItemsItem
      x-api-path-slug: itemsitemid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
---