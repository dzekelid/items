---
swagger: "2.0"
x-collection-name: eBay
x-complete: 1
info:
  title: Ebay
  description: the-ebay-platform-offers-an-unprecedented-opportunity-to-build-a-new-ebay-business-or-expand-your-current-business-reach-new-customers-and-create-a-potential-new-stream-of-revenue--leverage-the-resources-of-the-ebay-developers-program-to-tap-into-the-ebay-marketplace-with-millions-of-active-users-globally-with-tools-and-services-that-meet-the-diverse-needs-of-buyers-and-sellers-
  contact:
    name: eBay Inc.
  version: 1.0.0
host: api.ebay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /item/get_items_by_item_group:
    get:
      summary: Get Item Get Items By Item Group
      description: This call retrieves the details of the individual items in an item
        group. An item group is an item that has various aspect differences, such
        as color, size, storage capacity, etc. You pass in the item group Id as a
        URI parameter. You use this call to show the item details of items with multiple
        aspects, such as color, size, storage capacity, etc. This call returns two
        main containers; items and commonDescriptions. The items container has an
        array of containers with the details of each item in the group. The commonDescriptions
        container has an array of containers for a description and the item Ids of
        all the items that have this exact description. Because items within an item
        group often have the same description, this decreases the size of the response.
        Request headers You will want to use the X-EBAY-C-ENDUSERCTX request header
        with this call. If you are an eBay Network Partner you must use affiliateCampaignId=ePNCampaignId,affiliateReferenceId=referenceId
        in the header in order to be paid for selling eBay items on your site and
        it is strongly recommended you use contextualLocation to improved the estimated
        delivery window information. For details see, Request headers in the Buy APIs
        Overview. Restrictions For a list of supported sites and other restrictions,
        see API Restrictions.
      operationId: getItemsByItemGroup
      x-api-path-slug: itemget-items-by-item-group-get
      parameters:
      - in: query
        name: item_group_id
        description: Identifier of the item group to return
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Item
      - ""
      - Items
      - Item
      - Group
---