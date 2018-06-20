---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/payouts/{id}/line_items:
    get:
      summary: Get My Payouts Line Items
      description: Read the line items of a payout
      operationId: getMyPayoutsLineItems
      x-api-path-slug: mypayoutsidline-items-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Payouts
      - Id
      - Line
      - Items
---