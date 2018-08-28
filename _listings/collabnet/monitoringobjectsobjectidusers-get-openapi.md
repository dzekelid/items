---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Returns the list of monitoring users
    for the object(Folder/Item).
  version: 1.0.0
  description: Returns the list of monitoring users for the object(folder/item)..
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitoring/objects/{objectid}/users:
    get:
      summary: Returns the list of monitoring users for the object(Folder/Item).
      description: Returns the list of monitoring users for the object(folder/item)..
      operationId: listUsersForObject
      x-api-path-slug: monitoringobjectsobjectidusers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Usersthe
      - Object(Folder
      - Item)
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