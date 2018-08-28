---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Delete a related item by id for tags.
  version: 1.0.0
  description: Delete a related item by id for tags..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks/{id}/tags/{fk}:
    delete:
      summary: Delete a related item by id for tags.
      description: Delete a related item by id for tags..
      operationId: deleteDecksTagsFk
      x-api-path-slug: decksidtagsfk-delete
      parameters:
      - in: path
        name: fk
        description: Foreign key for tags
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Related
      - Item
      - By
      - Idtags
  /cards/{id}/tags/{fk}:
    delete:
      summary: Delete a related item by id for tags.
      description: Delete a related item by id for tags..
      operationId: deleteCardsTagsFk
      x-api-path-slug: cardsidtagsfk-delete
      parameters:
      - in: path
        name: fk
        description: Foreign key for tags
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Related
      - Item
      - By
      - Idtags
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