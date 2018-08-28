swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Xero oAuth 1a
  description: a-collection-to-authenticate-to-the-xero-api-using-oauth1-0a
  version: 1.0.0
host: api.xero.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Items:
    get:
      summary: Get Items
      description: Get items.
      operationId: getItems
      x-api-path-slug: items-get
      parameters:
      - in: query
        name: No Name
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Items
    post:
      summary: Post Items
      description: Post items.
      operationId: postItems
      x-api-path-slug: items-post
      parameters:
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
    put:
      summary: Put Items
      description: Put items.
      operationId: putItems
      x-api-path-slug: items-put
      parameters:
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
    x-related-model:
      summary: X-related-model Items
      description: X-related-model items.
      operationId: x-related-modelItems
      x-api-path-slug: items-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Items
  /Items/{ItemID}:
    delete:
      summary: Delete Items
      description: Delete items item.
      operationId: deleteItemsItem
      x-api-path-slug: itemsitemid-delete
      parameters:
      - in: path
        name: ItemID
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    get:
      summary: Get Items
      description: Get items item.
      operationId: getItemsItem
      x-api-path-slug: itemsitemid-get
      parameters:
      - in: path
        name: ItemID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    post:
      summary: Post Items
      description: Post items item.
      operationId: postItemsItem
      x-api-path-slug: itemsitemid-post
      parameters:
      - in: path
        name: ItemID
      - in: body
        name: Items
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID
    x-related-model:
      summary: X-related-model Items
      description: X-related-model items item.
      operationId: x-related-modelItemsItem
      x-api-path-slug: itemsitemid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Items
      - ItemID