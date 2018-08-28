swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
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