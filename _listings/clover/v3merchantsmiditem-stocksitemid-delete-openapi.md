---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Delete the stock of an inventory item
  version: 1.0.0
  description: Delete the stock of an inventory item.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/items:
    get:
      summary: Get all inventory items
      description: Get all inventory items.
      operationId: GetItems
      x-api-path-slug: v3merchantsmiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, sku, modifiedTime, deleted, hidden,
          price, alternateName, itemCode, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    post:
      summary: Create an inventory item
      description: Create an inventory item.
      operationId: CreateItem
      x-api-path-slug: v3merchantsmiditems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    delete:
      summary: Bulk delete inventory items
      description: Bulk delete inventory items.
      operationId: BulkDeleteItems
      x-api-path-slug: v3merchantsmiditems-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
  /v3/merchants/{mId}/items/{itemId}:
    get:
      summary: Get a single inventory item
      description: Get a single inventory item.
      operationId: GetItem
      x-api-path-slug: v3merchantsmiditemsitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    post:
      summary: Update an existing inventory item
      description: Update an existing inventory item.
      operationId: UpdateItem
      x-api-path-slug: v3merchantsmiditemsitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    delete:
      summary: Delete an inventory item
      description: Delete an inventory item.
      operationId: DeleteItem
      x-api-path-slug: v3merchantsmiditemsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
  /v3/merchants/{mId}/bulk_items:
    post:
      summary: Create multiple inventory items.
      description: This API is to create multiple inventory items.  Use the PATCH
        HTTP method to update existing inventory items.
      operationId: BulkCreateInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
      - Items
    put:
      summary: Update existing inventory items.
      description: This API is to going to update only the changes present in the
        payload. Not going to replace the existing inventory items. Use the POST HTTP
        method to create inventory items.
      operationId: BulkPatchInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items:
    get:
      summary: Get all line items for an order
      description: Get all line items for an order.
      operationId: GetOrderLineItems
      x-api-path-slug: v3merchantsmidordersorderidline-items-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
    post:
      summary: Create a new line item
      description: Create a new line item.
      operationId: CreateLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
  /v3/merchants/{mId}/items/{itemId}/tags:
    get:
      summary: Get tags for a single item
      description: Get tags for a single item.
      operationId: GetItemTags
      x-api-path-slug: v3merchantsmiditemsitemidtags-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Tags
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}:
    get:
      summary: Get a line item
      description: Get a line item.
      operationId: GetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    post:
      summary: Update a line item
      description: Update a line item.
      operationId: UpdateOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    delete:
      summary: Void a line item
      description: Void a line item.
      operationId: DeleteOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
  /v3/merchants/{mId}/tags/{tagId}/items:
    get:
      summary: Get all items for a single tag
      description: Get all items for a single tag.
      operationId: GetTaggedItems
      x-api-path-slug: v3merchantsmidtagstagiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, hidden, itemCode, alternateName,
          option'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
      - Items
  /v3/merchants/{mId}/tag_items:
    post:
      summary: Create or delete tag items
      description: Create or delete tag items.
      operationId: CreateOrDeleteTagItems
      x-api-path-slug: v3merchantsmidtag-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tag
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts:
    post:
      summary: Create a discount on an order or line item
      description: Create a discount on an order or line item.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts/{discountId}:
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: RemoveDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
      - DiscountId
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications:
    post:
      summary: Apply a modification to a line item
      description: 'Create a modification, a record of a modifier as it exists at
        the time it is applied to the lineItem. To view current modifications use
        an ''expand=modifications'' query parameter on the lineItem. To learn more
        about applying a modification see: https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
      operationId: ApplyModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications/{modificationId}:
    delete:
      summary: Remove a modification from a line item
      description: Delete a modification by UUID, removing the record of an applied
        modification
      operationId: RemoveModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modificationId
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
      - ModificationId
  /v3/merchants/{mId}/orders/{orderId}/bulk_line_items:
    post:
      summary: Create multiple line items in bulk.
      description: Create multiple line items in bulk..
      operationId: BulkCreateLineItems
      x-api-path-slug: v3merchantsmidordersorderidbulk-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Bulk
      - Line
      - Items
  /v3/merchants/{mId}/categories/{catId}/items:
    get:
      summary: Get all items in a single category
      description: Get all items in a single category.
      operationId: GetCategoryItems
      x-api-path-slug: v3merchantsmidcategoriescatiditems-get
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
      - Items
  /v3/merchants/{mId}/items/{itemId}/categories:
    get:
      summary: Get all categories of a single item
      description: Get all categories of a single item.
      operationId: GetItemCategories
      x-api-path-slug: v3merchantsmiditemsitemidcategories-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Categories
  /v3/merchants/{mId}/category_items:
    post:
      summary: Create or delete an item/category association
      description: Create or delete an item/category association.
      operationId: CreateOrDeleteCategoryItems
      x-api-path-slug: v3merchantsmidcategory-items-post
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Category
      - Items
  /v3/merchants/{mId}/tax_rate_items:
    post:
      summary: Create or delete a tax rate item
      description: Create or delete a tax rate item.
      operationId: CreateOrDeleteTaxRateItems
      x-api-path-slug: v3merchantsmidtax-rate-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rate
      - Items
  /v3/merchants/{mId}/tax_rates/{taxId}/items:
    get:
      summary: Get items by tax rate
      description: Get items by tax rate.
      operationId: GetItemsByTaxRate
      x-api-path-slug: v3merchantsmidtax-ratestaxiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, sku, modifiedTime, deleted, hidden,
          price, alternateName, itemCode, item'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: taxId
        description: Tax Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
      - TaxId
      - Items
  /v3/merchants/{mId}/orders/{orderId}/voided_line_items:
    post:
      summary: Void a line item
      description: Void a line item.
      operationId: VoidOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidvoided-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Voided
      - Line
      - Items
  /v3/merchants/{mId}/voided_line_items:
    get:
      summary: Get order line items that were recorded after a void
      description: Get order line items that were recorded after a void.
      operationId: GetVoidedOrderLineItems
      x-api-path-slug: v3merchantsmidvoided-line-items-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [reason, id, name, price, quantity, printed,
          deletedTime, merchantId, orderId, removedById]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Voided
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items/{oldLineItemId}/exchange/{lineItemId}:
    post:
      summary: Create or exchange a line item
      description: Create or exchange a line item.
      operationId: SetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: oldLineItemId
        description: Old Line Item Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - OldLineItemId
      - Exchange
      - LineItemId
  /v3/merchants/{mId}/option_items:
    post:
      summary: Create or delete item/option association
      description: See the description for 'get all item groups'.
      operationId: CreateOrDeleteOptionItems
      x-api-path-slug: v3merchantsmidoption-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Option
      - Items
  /v3/merchants/{mId}/item_stocks:
    get:
      summary: Get the stock of all inventory items
      description: Get the stock of all inventory items.
      operationId: GetItemStocks
      x-api-path-slug: v3merchantsmiditem-stocks-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
  /v3/merchants/{mId}/item_stocks/{itemId}:
    get:
      summary: Get the stock of an inventory item
      description: Get the stock of an inventory item.
      operationId: GetItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-get
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
    post:
      summary: Update the stock of an inventory item
      description: Update the stock of an inventory item.
      operationId: UpdateItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
    delete:
      summary: Delete the stock of an inventory item
      description: Delete the stock of an inventory item.
      operationId: DeleteItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-delete
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
  /v3/merchants/{mId}/item_groups:
    get:
      summary: Get all item groups
      description: |-
        Item Groups help merchants create and manage large groups of related items. This is described to merchants as an 'Item with variants'.

        For example a merchants may sell a t-shirt that is available in numerous various sizes and colors. Each of the t-shirt variations is an item and belongs to the t-shirt item group. Once an item group is created it appears in Register as a single button and tapping it brings up a choice of which variation is to be sold. Before adding items to an item group you first need to create the item group, then create attributes ('size', 'color') and then options for each attribute ('small', 'blue'), then associate options with an item and then associate items with an item group.

        The name of an item which is a member of an item group is automatically generated by the Clover server as a combination of the item group name and the name of all the options associated with that item. It cannot be changed. If the item group name is changed, or if an option name is changed, then the item names will be automatically regenerated.

        An item can only be a member of a single item group and once it is part of an item group it can never be removed or moved to another item group, it can only be deleted.
      operationId: GetItemGroups
      x-api-path-slug: v3merchantsmiditem-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, name, id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
    post:
      summary: Create an item group
      description: Create an item group.
      operationId: CreateItemGroup
      x-api-path-slug: v3merchantsmiditem-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
  /v3/merchants/{mId}/item_groups/{itemGroupId}:
    get:
      summary: Get a single item group
      description: Get a single item group.
      operationId: GetItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    post:
      summary: Update an item group
      description: Update an item group.
      operationId: UpdateItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    delete:
      summary: Delete an item group
      description: Delete an item group.
      operationId: DeleteItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-delete
      parameters:
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
  /v3/merchants/{mId}/item_modifier_groups:
    post:
      summary: Create or delete item to modifier group associations
      description: 'Create or delete one or more association objects (item modifier
        groups). Modifiers can only be applied to items associated with that modifier''s
        group. Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
      operationId: CreateOrDeleteItemModifierGroups
      x-api-path-slug: v3merchantsmiditem-modifier-groups-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Modifier
      - Groups
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