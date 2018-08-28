swagger: "2.0"
x-collection-name: 7digital
x-complete: 1
info:
  title: 7digital Purchasing API
  description: the-purchasing-api-allows-3rd-parties-to-deliver-digital-content-to-individual-users-
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  user/purchase/item:
    'get ':
      summary: user/purchase/item
      description: This method allows a user to purchase an item at the price as advertised
        on 7digital.com. It will return the download URL of each item purchased. For
        example, if a release consisting of multiple tracks was purchased, then the
        download URL of each item constituting the release will be returned.nttttttFor
        a user purchase to be processed, the user should already have a default debit
        or credit card set up for payments.ntttThis method allows users to take advantage
        of 7digital.com promotional offers and is only available to selected partners
        building 7digital branded integrations. For white-label integrations please
        use user/purchase/rrpItem or user/purchase/pricedItem.
      operationId: userpurchaseitem
      x-api-path-slug: userpurchaseitem-get
      parameters:
      - ~
      - in: query
        name: country
        description: The code of the country the end user resides in
      - in: query
        name: oauth_token
        description: users OAuth accesstoken
      - in: query
        name: price
        description: nttttttttThe price that has been displayed to the user prior
          to purchase
      - in: query
        name: releaseId
        description: The unique ID of the release being purchased
      - in: query
        name: shopid
        description: nttttttttThe shop ID that all basket items were selected from
      - in: query
        name: tag_*key*
        description: nttttttttAdditional data to be stored with successful transactions,
          for the purposes such as tagging affiliated or marketing information
      - in: query
        name: trackId
        description: The unique ID of the track being purchased
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - Item