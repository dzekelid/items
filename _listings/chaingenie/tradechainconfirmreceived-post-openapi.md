---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Delivery of item confirmed (by Buyer)
  description: "Delivery of item confirmed by the buyer \r\n-Escrow is fully sent
    to seller\r\n- End transaction state = TRANSACTION COMPLETE"
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tradechain/ConfirmReceived:
    post:
      summary: Delivery of item confirmed (by Buyer)
      description: "Delivery of item confirmed by the buyer \r\n-Escrow is fully sent
        to seller\r\n- End transaction state = TRANSACTION COMPLETE"
      operationId: TradechainConfirmReceivedPost
      x-api-path-slug: tradechainconfirmreceived-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemBuyerName
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delivery
      - Of
      - Item
      - Confirmed
      - (by
      - Buyer)
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