---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Modifies the details of an existing item category.
  description: Modifies the details of an existing item category.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/items:
    get:
      summary: Provides summary information for all of a location's items.
      description: Provides summary information for all of a location's items.
      operationId: ListItems
      x-api-path-slug: v1location-iditems-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: path
        name: location_id
        description: The ID of the location to list items for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Locations
      - Items
    post:
      summary: Creates an item and at least one variation for it.
      description: Creates an item and at least one variation for it.
      operationId: CreateItem
      x-api-path-slug: v1location-iditems-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - At
      - Least
      - Variationit
  /v1/{location_id}/categories:
    get:
      summary: Lists all of a location's item categories.
      description: Lists all of a location's item categories.
      operationId: ListCategories
      x-api-path-slug: v1location-idcategories-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Item
      - Categories
    post:
      summary: Creates an item category.
      description: Creates an item category.
      operationId: CreateCategory
      x-api-path-slug: v1location-idcategories-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Category
  /v1/{location_id}/categories/{category_id}:
    delete:
      summary: Deletes an existing item category.
      description: Deletes an existing item category.
      operationId: DeleteCategory
      x-api-path-slug: v1location-idcategoriescategory-id-delete
      parameters:
      - in: path
        name: category_id
        description: The ID of the category to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Category
    put:
      summary: Modifies the details of an existing item category.
      description: Modifies the details of an existing item category.
      operationId: UpdateCategory
      x-api-path-slug: v1location-idcategoriescategory-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: category_id
        description: The ID of the category to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Category
  /v1/{location_id}/inventory:
    get:
      summary: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      description: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      operationId: ListInventory
      x-api-path-slug: v1location-idinventory-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of inventory entries to return in a single
          response
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Inventory
      - Information
      - Of
      - Merchants
      - Inventory-enabled
      - Item
      - Variations
  /v1/{location_id}/inventory/{variation_id}:
    post:
      summary: Adjusts an item variation's current available inventory.
      description: Adjusts an item variation's current available inventory.
      operationId: AdjustInventory
      x-api-path-slug: v1location-idinventoryvariation-id-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to adjust inventory information for
      responses:
        200:
          description: OK
      tags:
      - Adjusts
      - Item
      - Variations
      - Current
      - Available
      - Inventory
  /v1/{location_id}/items/{item_id}:
    delete:
      summary: Deletes an existing item and all item variations associated with it.
      description: Deletes an existing item and all item variations associated with
        it.
      operationId: DeleteItem
      x-api-path-slug: v1location-iditemsitem-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - ""
      - Item
      - Variations
      - Associated
      - It
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
    put:
      summary: Modifies the core details of an existing item.
      description: Modifies the core details of an existing item.
      operationId: UpdateItem
      x-api-path-slug: v1location-iditemsitem-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Core
      - Details
      - Of
      - Existing
      - Item
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
    put:
      summary: Associates a fee with an item, meaning the fee is automatically applied
        to the item in Square Register.
      description: Associates a fee with an item, meaning the fee is automatically
        applied to the item in Square Register.
      operationId: ApplyFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-put
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Fee
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
  /v1/{location_id}/items/{item_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      description: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      operationId: RemoveModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to remove the modifier list from
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to remove
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Modifier
      - List
      - Association
      - From
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - "No"
      - Longer
      - Be
      - Applied
      - To
      - Item
    put:
      summary: Associates a modifier list with an item, meaning modifier options from
        the list can be applied to the item.
      description: Associates a modifier list with an item, meaning modifier options
        from the list can be applied to the item.
      operationId: ApplyModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to add the modifier list to
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to apply
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Modifier
      - List
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - Be
      - Applied
      - To
      - Item
  /v1/{location_id}/items/{item_id}/variations:
    post:
      summary: Creates an item variation for an existing item.
      description: Creates an item variation for an existing item.
      operationId: CreateVariation
      x-api-path-slug: v1location-iditemsitem-idvariations-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Variationan
      - Existing
      - Item
  /v1/{location_id}/items/{item_id}/variations/{variation_id}:
    delete:
      summary: Deletes an existing item variation from an item.
      description: Deletes an existing item variation from an item.
      operationId: DeleteVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Variation
      - From
      - Item
    put:
      summary: Modifies the details of an existing item variation.
      description: Modifies the details of an existing item variation.
      operationId: UpdateVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Variation
  /v1/{location_id}/modifier-lists:
    post:
      summary: Creates an item modifier list and at least one modifier option for
        it.
      description: Creates an item modifier list and at least one modifier option
        for it.
      operationId: CreateModifierList
      x-api-path-slug: v1location-idmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a modifier list for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - List
      - At
      - Least
      - Modifier
      - Optionit
  /v1/{location_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Deletes an existing item modifier list and all modifier options associated
        with it.
      description: Deletes an existing item modifier list and all modifier options
        associated with it.
      operationId: DeleteModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - List
      - ""
      - Modifier
      - Options
      - Associated
      - It
    put:
      summary: Modifies the details of an existing item modifier list.
      description: Modifies the details of an existing item modifier list.
      operationId: UpdateModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options:
    post:
      summary: Creates an item modifier option and adds it to a modifier list.
      description: Creates an item modifier option and adds it to a modifier list.
      operationId: CreateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptions-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - Option
      - Adds
      - It
      - To
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options/{modifier_option_id}:
    delete:
      summary: Deletes an existing item modifier option from a modifier list.
      description: Deletes an existing item modifier option from a modifier list.
      operationId: DeleteModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - Option
      - From
      - Modifier
      - List
    put:
      summary: Modifies the details of an existing item modifier option.
      description: Modifies the details of an existing item modifier option.
      operationId: UpdateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - Option
  /v2/catalog/update-item-modifier-lists:
    post:
      summary: UpdateItemModifierLists
      description: |-
        Updates the [CatalogModifierList](#type-catalogmodifierlist) objects
        that apply to the targeted [CatalogItem](#type-catalogitem) without having
        to perform an upsert on the entire item.
      operationId: UpdateItemModifierLists
      x-api-path-slug: v2catalogupdateitemmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ItemModifierLists
  /v2/catalog/update-item-taxes:
    post:
      summary: UpdateItemTaxes
      description: |-
        Updates the [CatalogTax](#type-catalogtax) objects that apply to the
        targeted [CatalogItem](#type-catalogitem) without having to perform an
        upsert on the entire item.
      operationId: UpdateItemTaxes
      x-api-path-slug: v2catalogupdateitemtaxes-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ItemTaxes
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