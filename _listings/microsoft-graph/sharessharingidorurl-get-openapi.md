---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Accessing Shared Drive Items
  description: Accessing shared DriveItems Access a shared DriveItem or a collection
    of shared items by using a shareId or sharing URL.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shares/{sharingIdOrUrl}:
    get:
      summary: Accessing Shared Drive Items
      description: Accessing shared DriveItems Access a shared DriveItem or a collection
        of shared items by using a shareId or sharing URL.
      operationId: AccessingSharedDriveItems
      x-api-path-slug: sharessharingidorurl-get
      parameters:
      - in: path
        name: sharingIdOrUrl
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accessing
      - Shared
      - Drive
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