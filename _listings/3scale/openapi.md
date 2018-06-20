---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 1
info:
  title: 3Scale Billing API
  description: the-api-for-managing-3scale-billing
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/invoices/{invoice_id}/line_items.xml:
    get:
      summary: Invoice Line Items List
      description: Invoice line items list.
      operationId: finance
      x-api-path-slug: apiinvoicesinvoice-idline-items-xml-get
      parameters:
      - in: path
        name: invoice_id
        description: id of the invoice
      - in: query
        name: provider_key
        description: Your api key with 3scale
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - Line
      - Items
      - List
---