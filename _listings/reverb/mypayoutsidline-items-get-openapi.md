---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get My Payouts Line Items
  description: Read the line items of a payout
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