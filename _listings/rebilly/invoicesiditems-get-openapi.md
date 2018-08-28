---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve invoice items
  description: Retrieve an invoice items with specified invoice identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /invoices/{id}/items:
    get:
      summary: Retrieve invoice items
      description: Retrieve an invoice items with specified invoice identifier string
      operationId: invoices.id.items.get
      x-api-path-slug: invoicesiditems-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Invoice
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