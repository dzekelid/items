swagger: "2.0"
x-collection-name: Blizzard
x-complete: 1
info:
  title: World of Warcraft
  description: welcome-to-the-restful-apis-exposed-through-the-world-of-warcraft-community-site-as-a-service-to-the-world-of-warcraft-community-
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