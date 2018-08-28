---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Updates a collection of items from a specific Order
  version: 1.0.0
  description: Updates a collection of items from a specific order.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/GiftRegistries/{giftregistryid}/Items:
    get:
      summary: Gets the items from a specific Gift Registry
      description: Gets the items from a specific gift registry.
      operationId: GiftRegistries_GetAllGiftRegistryItem
      x-api-path-slug: 3dcartwebapiv1giftregistriesgiftregistryiditems-get
      parameters:
      - in: path
        name: giftregistryid
        description: Gift Registry ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - Gift
      - Registry
  /3dCartWebAPI/v1/Orders/{orderid}/Items:
    get:
      summary: Gets the items from a specific Order
      description: Gets the items from a specific order.
      operationId: Orders_GetAllOrderItems
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of items from a specific Order
      description: Updates a collection of items from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-put
      parameters:
      - in: body
        name: items
        description: A Json or XML object containing the new items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Items
      - From
      - Specific
      - Order
    post:
      summary: Adds a new item on the order
      description: Adds a new item on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - "On"
      - Order
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling:
    put:
      summary: Updates a collection of upselling items from a specific Product
      description: Updates a collection of upselling items from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitems
        description: A Json or XML object containing the new upselling items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Upselling
      - Items
      - From
      - Specific
      - Product
    post:
      summary: Adds a new upselling item to the system
      description: Adds a new upselling item to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling item
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Upselling
      - Item
      - To
      - System
  /3dCartWebAPI/v1/RMA/{rmaid}/Items:
    get:
      summary: Gets the items from a specific RMA
      description: Gets the items from a specific rma.
      operationId: RMA_GetAllRMAItem
      x-api-path-slug: 3dcartwebapiv1rmarmaiditems-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: path
        name: rmaid
        description: Order ID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - RMA
  /3dCartWebAPI/v1/Cart/{orderkey}/Item:
    post:
      summary: Adds a new item to a cart
      description: Adds a new item to a cart.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitem-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - To
      - Cart
  /3dCartWebAPI/v1/Cart/{orderkey}/Item/{cartitemid}:
    put:
      summary: Updates a specific item from a specific Cart
      description: Updates a specific item from a specific cart.
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-put
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Cart
    delete:
      summary: Deletes a CartItem in the system
      description: Deletes a cartitem in the system.
      operationId: Carts_Delete
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-delete
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - CartItem
      - In
      - System
  /3dCartWebAPI/v1/Orders/{orderid}/Items/{itemindexid}:
    put:
      summary: Updates a specific item from a specific Product
      description: Updates a specific item from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditemsitemindexid-put
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemindexid
        description: The unique indexID of an Item
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling/{upsellingindexid}:
    put:
      summary: Updates a specific Upselling Item from a specific Product
      description: Updates a specific upselling item from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupsellingupsellingindexid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: path
        name: upsellingindexid
        description: UpSellingIndexID
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling tem
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Upselling
      - Item
      - From
      - Specific
      - Product
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