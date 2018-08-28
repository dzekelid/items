---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Get items in the product feed.
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Product/{partnerId}/{feedId}/Items:
    get:
      summary: Get items in the product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedItems
      x-api-path-slug: apiv1productpartneridfeediditems-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: query
        name: isCompliant
        description: Compliant filter
      - in: query
        name: page
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Items
      - In
      - Product
      - Feed
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