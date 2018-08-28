---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Delete User Ratings Itemtype Itemid
  description: This route deletes a given rating of a given type.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/ratings/{itemType}/{itemId}:
    delete:
      summary: Delete User Ratings Itemtype Itemid
      description: This route deletes a given rating of a given type.
      operationId: user.ratings.itemType.itemId.delete
      x-api-path-slug: userratingsitemtypeitemid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - ItemType
      - ItemId
  /user/ratings/{itemType}/{itemId}/{itemRating}:
    put:
      summary: Put User Ratings Itemtype Itemid Itemrating
      description: This route updates a given rating of a given type.
      operationId: user.ratings.itemType.itemId.itemRating.put
      x-api-path-slug: userratingsitemtypeitemiditemrating-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - ItemType
      - ItemId
      - ItemRating
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