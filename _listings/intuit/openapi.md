swagger: "2.0"
x-collection-name: Intuit
x-complete: 1
info:
  title: QuickBooks Online V3 API
  description: the-quickbooks-online-accounting-api-is-a-restful-api-that-is-used-to-access-quickbooks-companies-docs-
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /item:
    post:
      summary: Post Item
      description: |-
        Create an item object
        Method : POST
      operationId: postItem
      x-api-path-slug: item-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Item
  /reports/ItemSales:
    get:
      summary: Get Reports Item Sales
      description: |-
        Report - Item Sales
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/sales%20by%20product
      operationId: getReportsItemsales
      x-api-path-slug: reportsitemsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Item
      - Sales
  /item/<ID>:
    get:
      summary: Get Item
      description: |-
        Read an Item by Id
        Method : GET
      operationId: getItem<>
      x-api-path-slug: itemid-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Item