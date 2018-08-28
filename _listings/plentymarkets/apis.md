---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Items
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List basket items
  x-api-slug: restbasketitems-get
  description: Lists all items in the shopping cart for the current customer session.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitems-get-openapi.md
- name: plentymarkets REST-API - List all shipping profiles of all items
  x-api-slug: restitemsitem-shipping-profiles-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - Book out order items
  x-api-slug: restordersorderidoutgoing-stocks-post
  description: Books out the order items of an order. The ID of the order must be
    specified and a booking date can be specified. The current date and time will
    be used if no date is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-post-openapi.md
- name: plentymarkets REST-API - List item availabilities
  x-api-slug: restavailabilities-get
  description: Lists all item availabilities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilities-get-openapi.md
- name: plentymarkets REST-API - Get an item availability
  x-api-slug: restavailabilitiesid-get
  description: Gets an item availability. The ID of the availability must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-openapi.md
- name: plentymarkets REST-API - Update an item availability
  x-api-slug: restavailabilitiesid-put
  description: Updates an item availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-put-openapi.md
- name: plentymarkets REST-API - Add item to basket
  x-api-slug: restbasketitems-post
  description: Adds a new item to the shopping cart using the request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitems-post-openapi.md
- name: plentymarkets REST-API - Find a basket item by it's ID
  x-api-slug: restbasketitemsid-get
  description: Find a basket item by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitemsid-get-openapi.md
- name: plentymarkets REST-API - Delete item sets
  x-api-slug: restitem-sets-delete
  description: Delete item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-openapi.md
- name: plentymarkets REST-API - List item sets
  x-api-slug: restitem-sets-get
  description: Lists all item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-openapi.md
- name: plentymarkets REST-API - Create item sets
  x-api-slug: restitem-sets-post
  description: Create item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-openapi.md
- name: plentymarkets REST-API - Update item sets
  x-api-slug: restitem-sets-put
  description: Update item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-openapi.md
- name: plentymarkets REST-API - Delete an item set
  x-api-slug: restitem-setsid-delete
  description: Deletes an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-delete-openapi.md
- name: plentymarkets REST-API - Get an item set
  x-api-slug: restitem-setsid-get
  description: Gets the configuration of an item set. The item ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-get-openapi.md
- name: plentymarkets REST-API - Update an item set
  x-api-slug: restitem-setsid-put
  description: Updates an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-put-openapi.md
- name: plentymarkets REST-API - Delete item set components
  x-api-slug: restitem-setssetidcomponents-delete
  description: Delete item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-openapi.md
- name: plentymarkets REST-API - List item set components of an item set
  x-api-slug: restitem-setssetidcomponents-get
  description: Lists the item set components of an item set. The ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-openapi.md
- name: plentymarkets REST-API - Create item set components
  x-api-slug: restitem-setssetidcomponents-post
  description: Create item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-openapi.md
- name: plentymarkets REST-API - Update item set components
  x-api-slug: restitem-setssetidcomponents-put
  description: Update item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-openapi.md
- name: plentymarkets REST-API - Delete an item set component
  x-api-slug: restitem-setssetidcomponentsid-delete
  description: Deletes an item set component. The item set component ID of the item
    set component must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-openapi.md
- name: plentymarkets REST-API - Get an item set component
  x-api-slug: restitem-setssetidcomponentsid-get
  description: Get an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-openapi.md
- name: plentymarkets REST-API - Update an item set component
  x-api-slug: restitem-setssetidcomponentsid-put
  description: Update an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Search item
  x-api-slug: restitems-get
  description: Search item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-get-openapi.md
- name: plentymarkets REST-API - Create new item
  x-api-slug: restitems-post
  description: Create new item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-post-openapi.md
- name: plentymarkets REST-API - List item label templates
  x-api-slug: restitemslabels-get
  description: Lists the ID and name of all item label templates saved in the system.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemslabels-get-openapi.md
- name: plentymarkets REST-API - List images of an item
  x-api-slug: restitemsidimages-get
  description: Lists all images of an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidimages-get-openapi.md
- name: plentymarkets REST-API - List image links of an item
  x-api-slug: restitemsidvariation-images-get
  description: Lists all images linked to an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidvariation-images-get-openapi.md
- name: plentymarkets REST-API - Delete an item
  x-api-slug: restitemsitemid-delete
  description: Deletes an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-delete-openapi.md
- name: plentymarkets REST-API - Show an item
  x-api-slug: restitemsitemid-get
  description: Show an item by itemId
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-get-openapi.md
- name: plentymarkets REST-API - Update a item
  x-api-slug: restitemsitemid-put
  description: Updates a item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-put-openapi.md
- name: plentymarkets REST-API - Deactivate shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-delete
  description: Deactivates all shipping profiles of an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-openapi.md
- name: plentymarkets REST-API - List shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-get
  description: Lists the shipping profiles linked to an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - List variations of an item
  x-api-slug: restitemsitemidvariations-get
  description: Lists all variations of an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemidvariations-get-openapi.md
- name: plentymarkets REST-API - List item specifics
  x-api-slug: restmarketsebayitem-specifics-get
  description: List item specifics for a given category Id and referrerId.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restmarketsebayitem-specifics-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - List item availabilities
  x-api-slug: restavailabilities-get
  description: Lists all item availabilities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilities-get-openapi.md
- name: plentymarkets REST-API - Get an item availability
  x-api-slug: restavailabilitiesid-get
  description: Gets an item availability. The ID of the availability must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-openapi.md
- name: plentymarkets REST-API - Update an item availability
  x-api-slug: restavailabilitiesid-put
  description: Updates an item availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-put-openapi.md
- name: plentymarkets REST-API - Add item to basket
  x-api-slug: restbasketitems-post
  description: Adds a new item to the shopping cart using the request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitems-post-openapi.md
- name: plentymarkets REST-API - Find a basket item by it's ID
  x-api-slug: restbasketitemsid-get
  description: Find a basket item by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitemsid-get-openapi.md
- name: plentymarkets REST-API - Delete item sets
  x-api-slug: restitem-sets-delete
  description: Delete item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-openapi.md
- name: plentymarkets REST-API - List item sets
  x-api-slug: restitem-sets-get
  description: Lists all item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-openapi.md
- name: plentymarkets REST-API - Create item sets
  x-api-slug: restitem-sets-post
  description: Create item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-openapi.md
- name: plentymarkets REST-API - Update item sets
  x-api-slug: restitem-sets-put
  description: Update item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-openapi.md
- name: plentymarkets REST-API - Delete an item set
  x-api-slug: restitem-setsid-delete
  description: Deletes an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-delete-openapi.md
- name: plentymarkets REST-API - Get an item set
  x-api-slug: restitem-setsid-get
  description: Gets the configuration of an item set. The item ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-get-openapi.md
- name: plentymarkets REST-API - Update an item set
  x-api-slug: restitem-setsid-put
  description: Updates an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-put-openapi.md
- name: plentymarkets REST-API - Delete item set components
  x-api-slug: restitem-setssetidcomponents-delete
  description: Delete item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-openapi.md
- name: plentymarkets REST-API - List item set components of an item set
  x-api-slug: restitem-setssetidcomponents-get
  description: Lists the item set components of an item set. The ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-openapi.md
- name: plentymarkets REST-API - Create item set components
  x-api-slug: restitem-setssetidcomponents-post
  description: Create item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-openapi.md
- name: plentymarkets REST-API - Update item set components
  x-api-slug: restitem-setssetidcomponents-put
  description: Update item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-openapi.md
- name: plentymarkets REST-API - Delete an item set component
  x-api-slug: restitem-setssetidcomponentsid-delete
  description: Deletes an item set component. The item set component ID of the item
    set component must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-openapi.md
- name: plentymarkets REST-API - Get an item set component
  x-api-slug: restitem-setssetidcomponentsid-get
  description: Get an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-openapi.md
- name: plentymarkets REST-API - Update an item set component
  x-api-slug: restitem-setssetidcomponentsid-put
  description: Update an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Search item
  x-api-slug: restitems-get
  description: Search item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-get-openapi.md
- name: plentymarkets REST-API - Create new item
  x-api-slug: restitems-post
  description: Create new item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-post-openapi.md
- name: plentymarkets REST-API - List item label templates
  x-api-slug: restitemslabels-get
  description: Lists the ID and name of all item label templates saved in the system.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemslabels-get-openapi.md
- name: plentymarkets REST-API - List images of an item
  x-api-slug: restitemsidimages-get
  description: Lists all images of an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidimages-get-openapi.md
- name: plentymarkets REST-API - List image links of an item
  x-api-slug: restitemsidvariation-images-get
  description: Lists all images linked to an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidvariation-images-get-openapi.md
- name: plentymarkets REST-API - Delete an item
  x-api-slug: restitemsitemid-delete
  description: Deletes an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-delete-openapi.md
- name: plentymarkets REST-API - Show an item
  x-api-slug: restitemsitemid-get
  description: Show an item by itemId
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-get-openapi.md
- name: plentymarkets REST-API - Update a item
  x-api-slug: restitemsitemid-put
  description: Updates a item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-put-openapi.md
- name: plentymarkets REST-API - Deactivate shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-delete
  description: Deactivates all shipping profiles of an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-openapi.md
- name: plentymarkets REST-API - List shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-get
  description: Lists the shipping profiles linked to an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - List variations of an item
  x-api-slug: restitemsitemidvariations-get
  description: Lists all variations of an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemidvariations-get-openapi.md
- name: plentymarkets REST-API - List item specifics
  x-api-slug: restmarketsebayitem-specifics-get
  description: List item specifics for a given category Id and referrerId.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restmarketsebayitem-specifics-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - List item specifics
  x-api-slug: restmarketsebayitem-specifics-get
  description: List item specifics for a given category Id and referrerId.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restmarketsebayitem-specifics-get-openapi.md
- name: plentymarkets REST-API - List variations of an item
  x-api-slug: restitemsitemidvariations-get
  description: Lists all variations of an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemidvariations-get-openapi.md
- name: plentymarkets REST-API - List shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-get
  description: Lists the shipping profiles linked to an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - Deactivate shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-delete
  description: Deactivates all shipping profiles of an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-openapi.md
- name: plentymarkets REST-API - Update a item
  x-api-slug: restitemsitemid-put
  description: Updates a item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-put-openapi.md
- name: plentymarkets REST-API - Show an item
  x-api-slug: restitemsitemid-get
  description: Show an item by itemId
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-get-openapi.md
- name: plentymarkets REST-API - Delete an item
  x-api-slug: restitemsitemid-delete
  description: Deletes an item. The ID of the item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsitemid-delete-openapi.md
- name: plentymarkets REST-API - List image links of an item
  x-api-slug: restitemsidvariation-images-get
  description: Lists all images linked to an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidvariation-images-get-openapi.md
- name: plentymarkets REST-API - List images of an item
  x-api-slug: restitemsidimages-get
  description: Lists all images of an item. The item ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemsidimages-get-openapi.md
- name: plentymarkets REST-API - List item label templates
  x-api-slug: restitemslabels-get
  description: Lists the ID and name of all item label templates saved in the system.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitemslabels-get-openapi.md
- name: plentymarkets REST-API - Create new item
  x-api-slug: restitems-post
  description: Create new item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-post-openapi.md
- name: plentymarkets REST-API - Search item
  x-api-slug: restitems-get
  description: Search item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitems-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Update an item set component
  x-api-slug: restitem-setssetidcomponentsid-put
  description: Update an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-put-openapi.md
- name: plentymarkets REST-API - Get an item set component
  x-api-slug: restitem-setssetidcomponentsid-get
  description: Get an item set component.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-get-openapi.md
- name: plentymarkets REST-API - Delete an item set component
  x-api-slug: restitem-setssetidcomponentsid-delete
  description: Deletes an item set component. The item set component ID of the item
    set component must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponentsid-delete-openapi.md
- name: plentymarkets REST-API - Update item set components
  x-api-slug: restitem-setssetidcomponents-put
  description: Update item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-put-openapi.md
- name: plentymarkets REST-API - Create item set components
  x-api-slug: restitem-setssetidcomponents-post
  description: Create item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-post-openapi.md
- name: plentymarkets REST-API - List item set components of an item set
  x-api-slug: restitem-setssetidcomponents-get
  description: Lists the item set components of an item set. The ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-get-openapi.md
- name: plentymarkets REST-API - Delete item set components
  x-api-slug: restitem-setssetidcomponents-delete
  description: Delete item set components.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setssetidcomponents-delete-openapi.md
- name: plentymarkets REST-API - Update an item set
  x-api-slug: restitem-setsid-put
  description: Updates an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-put-openapi.md
- name: plentymarkets REST-API - Get an item set
  x-api-slug: restitem-setsid-get
  description: Gets the configuration of an item set. The item ID of the item set
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-get-openapi.md
- name: plentymarkets REST-API - Delete an item set
  x-api-slug: restitem-setsid-delete
  description: Deletes an item set. The item ID of the item set must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-setsid-delete-openapi.md
- name: plentymarkets REST-API - Update item sets
  x-api-slug: restitem-sets-put
  description: Update item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-put-openapi.md
- name: plentymarkets REST-API - Create item sets
  x-api-slug: restitem-sets-post
  description: Create item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-post-openapi.md
- name: plentymarkets REST-API - List item sets
  x-api-slug: restitem-sets-get
  description: Lists all item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-get-openapi.md
- name: plentymarkets REST-API - Delete item sets
  x-api-slug: restitem-sets-delete
  description: Delete item sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restitem-sets-delete-openapi.md
- name: plentymarkets REST-API - Find a basket item by it's ID
  x-api-slug: restbasketitemsid-get
  description: Find a basket item by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitemsid-get-openapi.md
- name: plentymarkets REST-API - Add item to basket
  x-api-slug: restbasketitems-post
  description: Adds a new item to the shopping cart using the request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restbasketitems-post-openapi.md
- name: plentymarkets REST-API - Update an item availability
  x-api-slug: restavailabilitiesid-put
  description: Updates an item availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-put-openapi.md
- name: plentymarkets REST-API - Get an item availability
  x-api-slug: restavailabilitiesid-get
  description: Gets an item availability. The ID of the availability must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilitiesid-get-openapi.md
- name: plentymarkets REST-API - List item availabilities
  x-api-slug: restavailabilities-get
  description: Lists all item availabilities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/plentymarkets/restavailabilities-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---