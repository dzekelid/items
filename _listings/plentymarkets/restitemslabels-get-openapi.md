---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List item label templates
  description: Lists the ID and name of all item label templates saved in the system.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/basket/items:
    get:
      summary: List basket items
      description: Lists all items in the shopping cart for the current customer session.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitems-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Basket
      - Items
    post:
      summary: Add item to basket
      description: Adds a new item to the shopping cart using the request parameters.
      operationId: postRestBasketItems
      x-api-path-slug: restbasketitems-post
      parameters:
      - in: body
        name: /rest/basket/items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Item
      - To
      - Basket
  /rest/items/item_shipping_profiles:
    get:
      summary: List all shipping profiles of all items
      description: |-
        Lists all shipping profiles of all items. Results can be filtered by the timestamp of the link between items and shipping profiles (eq, lt, lte, gt, gte, between).
        <ul>
        <li>eq = Equal to</li>
        <li>gte = Greater than or equal to</li>
        <li>gt = Greater than</li>
        <li>lte = Less than or equal to</li>
        <li>lt = Less than</li>
        <li>between = Date range</li>
        </ul>
        Example: updated=gt:2018-04-16 16:00:00 returns all items with shipping profiles that were activated after 4pm on the 16th of April 2018.
      operationId: getRestItemsItemShippingProfiles
      x-api-path-slug: restitemsitem-shipping-profiles-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Shipping
      - Profiles
      - Of
      - ""
      - Items
  /rest/orders/{orderId}/outgoing_stocks:
    post:
      summary: Book out order items
      description: Books out the order items of an order. The ID of the order must
        be specified and a booking date can be specified. The current date and time
        will be used if no date is specified.
      operationId: postRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-post
      parameters:
      - in: query
        name: date
        description: The date that is saved as booking date for the outgoing stock
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Out
      - Order
      - Items
  /rest/availabilities:
    get:
      summary: List item availabilities
      description: Lists all item availabilities.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilities-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Availabilities
  /rest/availabilities/{id}:
    get:
      summary: Get an item availability
      description: Gets an item availability. The ID of the availability must be specified.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilitiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
    put:
      summary: Update an item availability
      description: Updates an item availability.
      operationId: putRestAvailabilities
      x-api-path-slug: restavailabilitiesid-put
      parameters:
      - in: body
        name: /rest/availabilities/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
  /rest/basket/items/{id}:
    get:
      summary: Find a basket item by it's ID
      description: Find a basket item by it's id.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitemsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Basket
      - Item
      - By
      - Its
      - ID
  /rest/item_sets:
    delete:
      summary: Delete item sets
      description: Delete item sets.
      operationId: deleteRestItemSets
      x-api-path-slug: restitem-sets-delete
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
    get:
      summary: List item sets
      description: Lists all item sets.
      operationId: getRestItemSets
      x-api-path-slug: restitem-sets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Sets
    post:
      summary: Create item sets
      description: Create item sets.
      operationId: postRestItemSets
      x-api-path-slug: restitem-sets-post
      parameters:
      - in: query
        name: params
        description: includes the item sets that have to be created
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
    put:
      summary: Update item sets
      description: Update item sets.
      operationId: putRestItemSets
      x-api-path-slug: restitem-sets-put
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
  /rest/item_sets/{id}:
    delete:
      summary: Delete an item set
      description: Deletes an item set. The item ID of the item set must be specified.
      operationId: deleteRestItemSets
      x-api-path-slug: restitem-setsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
    get:
      summary: Get an item set
      description: Gets the configuration of an item set. The item ID of the item
        set must be specified.
      operationId: getRestItemSets
      x-api-path-slug: restitem-setsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
    put:
      summary: Update an item set
      description: Updates an item set. The item ID of the item set must be specified.
      operationId: putRestItemSets
      x-api-path-slug: restitem-setsid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
  /rest/item_sets/{setId}/components:
    delete:
      summary: Delete item set components
      description: Delete item set components.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-delete
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
    get:
      summary: List item set components of an item set
      description: Lists the item set components of an item set. The ID of the item
        set must be specified.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Set
      - Components
      - Of
      - Item
      - Set
    post:
      summary: Create item set components
      description: Create item set components.
      operationId: postRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-post
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
    put:
      summary: Update item set components
      description: Update item set components.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
  /rest/item_sets/{setId}/components/{id}:
    delete:
      summary: Delete an item set component
      description: Deletes an item set component. The item set component ID of the
        item set component must be specified.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    get:
      summary: Get an item set component
      description: Get an item set component.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    put:
      summary: Update an item set component
      description: Update an item set component.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
  /rest/item_sets/{setId}/config:
    get:
      summary: Get the item set configuration of an item set
      description: Get the item set configuration of an item set.
      operationId: getRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
      - Of
      - Item
      - Set
    put:
      summary: Update an item set configuration
      description: Update an item set configuration.
      operationId: putRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
  /rest/items:
    get:
      summary: Search item
      description: Search item.
      operationId: getRestItems
      x-api-path-slug: restitems-get
      parameters:
      - in: query
        name: flagOne
        description: Filter restricts the list of results to items with the specified
          flagOne
      - in: query
        name: flagTwo
        description: Filter restricts the list of results to items with the specified
          flagTwo
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to items with the specified
          manufacturerId
      - in: query
        name: name
        description: Filter restricts the list of results to items with the specified
          item name
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: tagId
        description: Filter restricts the list of results to items with the specified
          tagId
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to items updated during
          the specified period
      - in: query
        name: variationRelatedUpdatedBetween
        description: Filter restricts the list of results to items with variations
          for which related information was updated during the specified period
      - in: query
        name: variationUpdatedBetween
        description: Filter restricts the list of results to items with variations
          that were updated during the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Item
    post:
      summary: Create new item
      description: Create new item.
      operationId: postRestItems
      x-api-path-slug: restitems-post
      parameters:
      - in: body
        name: /rest/items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Item
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
      - Templates
  /rest/items/{id}/images:
    get:
      summary: List images of an item
      description: Lists all images of an item. The item ID must be specified.
      operationId: getRestItemsImages
      x-api-path-slug: restitemsidimages-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
      - Of
      - Item
  /rest/items/{id}/variation_images:
    get:
      summary: List image links of an item
      description: Lists all images linked to an item. The item ID must be specified.
      operationId: getRestItemsVariationImages
      x-api-path-slug: restitemsidvariation-images-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Item
  /rest/items/{itemId}:
    delete:
      summary: Delete an item
      description: Deletes an item. The ID of the item must be specified.
      operationId: deleteRestItemsItem
      x-api-path-slug: restitemsitemid-delete
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Item
    get:
      summary: Show an item
      description: Show an item by itemId
      operationId: getRestItemsItem
      x-api-path-slug: restitemsitemid-get
      parameters:
      - in: path
        name: itemId
      - in: query
        name: lang
        description: The language of the variation information
      responses:
        200:
          description: OK
      tags:
      - Show
      - Item
    put:
      summary: Update a item
      description: Updates a item. The ID of the item must be specified.
      operationId: putRestItemsItem
      x-api-path-slug: restitemsitemid-put
      parameters:
      - in: body
        name: /rest/items/{itemId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Item
  /rest/items/{itemId}/item_shipping_profiles:
    delete:
      summary: Deactivate shipping profiles of an item
      description: Deactivates all shipping profiles of an item. The ID of the item
        must be specified.
      operationId: deleteRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-delete
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Shipping
      - Profiles
      - Of
      - Item
    get:
      summary: List shipping profiles of an item
      description: Lists the shipping profiles linked to an item. The ID of the item
        must be specified.
      operationId: getRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-get
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Profiles
      - Of
      - Item
  /rest/items/{itemId}/variations:
    get:
      summary: List variations of an item
      description: Lists all variations of an item. The ID of the item must be specified.
      operationId: getRestItemsItemVariations
      x-api-path-slug: restitemsitemidvariations-get
      parameters:
      - in: query
        name: barcode
        description: Filter restricts the list of results to variations with the specified
          barcode
      - in: query
        name: createdBetween
        description: Filter restricts the list of results to variations created during
          the specified period
      - in: query
        name: isActive
        description: Filter restricts the list of results to variations that are active
      - in: query
        name: isBundle
        description: Filter restricts the list of results to variations to which variations
          were added to create a bundle
      - in: query
        name: isMain
        description: Filter restricts the list of results to variations that are main
          variations
      - in: path
        name: itemId
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to variations with the specified
          manufacturer ID
      - in: query
        name: numberExact
        description: Filter restricts the list of results to the variation with the
          variation number specified
      - in: query
        name: numberFuzzy
        description: Filter restricts the list of results to variations with numbers
          that contain the variation number specified (SQL LIKE operator)
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: relatedUpdatedBetween
        description: Filter restricts the list of results to those variations for
          which related information was updated during the specified period
      - in: query
        name: supplierNumber
        description: Filter restricts the list of results to variations with the specified
          supplier number
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to variations updated during
          the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Variations
      - Of
      - Item
  /rest/markets/ebay/item_specifics:
    get:
      summary: List item specifics
      description: List item specifics for a given category Id and referrerId.
      operationId: getRestMarketsEbayItemSpecifics
      x-api-path-slug: restmarketsebayitem-specifics-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category for which to list item specifics
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Specifics
  /rest/orders/items/dates:
    post:
      summary: Create a date for an order item
      description: Creates a date for an order item. The ID of the order item must
        be specified
      operationId: postRestOrdersItemsDates
      x-api-path-slug: restordersitemsdates-post
      parameters:
      - in: body
        name: /rest/orders/items/dates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
  /rest/orders/items/dates/{id}:
    delete:
      summary: Delete a date from an order item
      description: Deletes the date from an order item. The ID of the date must be
        specified.
      operationId: deleteRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
    get:
      summary: Get a date of an order item
      description: Gets a date of an order item. The ID of the date must be specified.
      operationId: getRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
    put:
      summary: Update a date of an order item
      description: Updates a date of an order item. The ID of the date must be specified.
      operationId: putRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-put
      parameters:
      - in: body
        name: /rest/orders/items/dates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
  /rest/orders/items/properties:
    post:
      summary: Create an order item property.
      description: Create an order item property..
      operationId: postRestOrdersItemsProperties
      x-api-path-slug: restordersitemsproperties-post
      parameters:
      - in: body
        name: /rest/orders/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
  /rest/orders/items/properties/{id}:
    delete:
      summary: Delete an order item property by ID.
      description: Delete an order item property by id..
      operationId: deleteRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    get:
      summary: Get an order item property by ID.
      description: Get an order item property by id..
      operationId: getRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    put:
      summary: Update an order item property by ID.
      description: Update an order item property by id..
      operationId: putRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
  /rest/orders/items/{orderItemId}/dates:
    get:
      summary: List dates of an order item
      description: Lists the dates of an order item. The ID of the order item must
        be specified.
      operationId: getRestOrdersItemsOrderitemDates
      x-api-path-slug: restordersitemsorderitemiddates-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
      - Item
  /rest/orders/items/{orderItemId}/dates/{typeId}:
    delete:
      summary: Delete a date from an order item by order item and date type
      description: Deletest a date from an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: deleteRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    get:
      summary: Get a date of an order item by order item and date type
      description: Gets a date of an order item. The ID of the order item and the
        ID of the date type must be specified.
      operationId: getRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    post:
      summary: Create a date for an order item by order item and date type
      description: Creates a date for an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: postRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    put:
      summary: Update a date of an order item by order item and date type
      description: Updates the date of an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: putRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
  /rest/orders/items/{orderItemId}/properties:
    get:
      summary: Get all order item propertys for one order item by its order item id.
      description: Get all order item propertys for one order item by its order item
        id..
      operationId: getRestOrdersItemsOrderitemProperties
      x-api-path-slug: restordersitemsorderitemidproperties-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Propertysone
      - Order
      - Item
      - By
      - Its
      - Order
      - Item
      - Id
  /rest/orders/items/{orderItemId}/properties/{typeId}:
    delete:
      summary: Delete an order item property by order item ID and order property type
        ID.
      description: Delete an order item property by order item id and order property
        type id..
      operationId: deleteRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    get:
      summary: Get an order item property by order item ID and order property type
        ID.
      description: Get an order item property by order item id and order property
        type id..
      operationId: getRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    post:
      summary: Create an order item property by order item ID and order property type
        ID.
      description: Create an order item property by order item id and order property
        type id..
      operationId: postRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    put:
      summary: Update an order item property by order item ID and order property type
        ID.
      description: Update an order item property by order item id and order property
        type id..
      operationId: putRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
  /rest/orders/{orderId}/items/{orderItemId}:
    delete:
      summary: Delete an order item
      description: Deletes an order item. The ID of the order and the ID of the order
        item must be specified.
      operationId: deleteRestOrdersOrderItemsOrderitem
      x-api-path-slug: restordersorderiditemsorderitemid-delete
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
  /rest/orders/{orderId}/items/{orderItemId}/serialNumbers:
    get:
      summary: List serial numbers of an order item
      description: Lists all serial numbers of an order item. The ID of the order
        and the ID of the order item must be specified.
      operationId: getRestOrdersOrderItemsOrderitemSerialnumbers
      x-api-path-slug: restordersorderiditemsorderitemidserialnumbers-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
      - Item
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