---
swagger: "2.0"
x-collection-name: Blizzard
x-complete: 0
info:
  title: World of Warcraft Get Data Item Classes
  description: Provides a list of item classes.
  version: 1.0.0
host: us.battle.net
basePath: /api/wow/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /item/{itemId}:
    get:
      summary: Get Item Itemid
      description: Provides detailed item information.
      operationId: getItemItem
      x-api-path-slug: itemitemid-get
      parameters:
      - in: path
        name: itemId
        description: The item ID
      responses:
        200:
          description: OK
      tags:
      - Item
      - ItemId
  /data/item/classes:
    get:
      summary: Get Data Item Classes
      description: Provides a list of item classes.
      operationId: getDataItemClasses
      x-api-path-slug: dataitemclasses-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Item
      - Classes
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