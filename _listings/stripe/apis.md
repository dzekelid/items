---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripes payment platform to accept
  and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1914"
tags: Items
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Get Invoiceitems
  x-api-slug: stripe
  description: Returns a list of your invoice items. Invoice items are returned sorted
    by creation date, with the most recently created invoice items appearing first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///invoiceitems
  tags: Invoiceitems
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/invoiceitems-get-openapi.md
- name: Stripe Add Invoiceitems
  x-api-slug: stripe
  description: "Adds an arbitrary charge or credit to the customer\u2019s upcoming
    invoice."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///invoiceitems
  tags: Invoiceitems
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/invoiceitems-post-openapi.md
- name: Stripe Delete Invoiceitems Invoiceitem
  x-api-slug: stripe
  description: "Removes an invoice item from the upcoming invoice. Removing an invoice
    item is only possible before the invoice it\u2019s attached to is closed."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///invoiceitems/{invoiceitem}
  tags: Invoiceitems, Invoiceitem
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/invoiceitemsinvoiceitem-delete-openapi.md
- name: Stripe Get Invoiceitems Invoiceitem
  x-api-slug: stripe
  description: Retrieves the invoice item with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///invoiceitems/{invoiceitem}
  tags: Invoiceitems, Invoiceitem
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/invoiceitemsinvoiceitem-get-openapi.md
- name: Stripe Add Invoiceitems Invoiceitem
  x-api-slug: stripe
  description: "Updates the amount or description of an invoice item on an upcoming
    invoice. Updating an invoice item is only possible before the invoice it\u2019s
    attached to is closed."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///invoiceitems/{invoiceitem}
  tags: Invoiceitems, Invoiceitem
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/invoiceitemsinvoiceitem-post-openapi.md
- name: Stripe Get Subscription Items
  x-api-slug: stripe
  description: Returns a list of your subscription items for a given subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscription_items
  tags: Subscription, Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/subscription-items-get-openapi.md
- name: Stripe Add Subscription Items
  x-api-slug: stripe
  description: Adds a new item to an existing subscription. No existing items will
    be changed or replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscription_items
  tags: Subscription, Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/subscription-items-post-openapi.md
- name: Stripe Delete Subscription Items Item
  x-api-slug: stripe
  description: Deletes an item from the subscription. Removing a subscription item
    from a subscription will not cancel the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscription_items/{item}
  tags: Subscription, Items, Item
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/subscription-itemsitem-delete-openapi.md
- name: Stripe Get Subscription Items Item
  x-api-slug: stripe
  description: Retrieves the invoice item with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscription_items/{item}
  tags: Subscription, Items, Item
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/subscription-itemsitem-get-openapi.md
- name: Stripe Add Subscription Items Item
  x-api-slug: stripe
  description: Updates the plan or quantity of an item on a current subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscription_items/{item}
  tags: Subscription, Items, Item
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/subscription-itemsitem-post-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/stripe/openapi.md
x-common:
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-email
  url: dpo@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-linkedin
  url: https://www.linkedin.com/company/stripe/
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---