---
name: eBay
x-slug: ebay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
x-kinRank: "8"
x-alexaRank: "42"
tags: Items
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/ebay/apis.md
specificationVersion: "0.14"
apis:
- name: Ebay Get Item Get Items By Item Group
  x-api-slug: ebay
  description: This call retrieves the details of the individual items in an item
    group. An item group is an item that has various aspect differences, such as color,
    size, storage capacity, etc. You pass in the item group Id as a URI parameter.
    You use this call to show the item details of items with multiple aspects, such
    as color, size, storage capacity, etc. This call returns two main containers;
    items and commonDescriptions. The items container has an array of containers with
    the details of each item in the group. The commonDescriptions container has an
    array of containers for a description and the item Ids of all the items that have
    this exact description. Because items within an item group often have the same
    description, this decreases the size of the response. Request headers You will
    want to use the X-EBAY-C-ENDUSERCTX request header with this call. If you are
    an eBay Network Partner you must use affiliateCampaignId=ePNCampaignId,affiliateReferenceId=referenceId
    in the header in order to be paid for selling eBay items on your site and it is
    strongly recommended you use contextualLocation to improved the estimated delivery
    window information. For details see, Request headers in the Buy APIs Overview.
    Restrictions For a list of supported sites and other restrictions, see API Restrictions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com////item/get_items_by_item_group
  tags: Auctions,Item, , Items, Item, Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/ebay/itemget-items-by-item-group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/ebay/itemget-items-by-item-group-get-openapi.md
- name: Ebay
  x-api-slug: ebay
  description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
    goods, digital cameras, baby items, coupons, and everything else on eBay, the
    worlds online marketplace
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/ebay/openapi.md
x-common:
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-crunchbase
  url: https://crunchbase.com/organization/leah
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-email
  url: spam@ebay.com
- type: x-email
  url: spoof@ebay.com
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/eBay
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---