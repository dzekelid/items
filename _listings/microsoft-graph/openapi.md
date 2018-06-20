---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
---