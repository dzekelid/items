---
swagger: "2.0"
x-collection-name: Stripe
x-complete: 0
info:
  title: Stripe Get Subscription Items
  description: Returns a list of your subscription items for a given subscription.
  termsOfService: https://stripe.com/us/terms/
  contact:
    name: Stripe Dev Platform Team
    url: https://stripe.com
    email: dev-platform@stripe.com
  version: v1
host: api.stripe.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /invoiceitems:
    get:
      summary: Get Invoiceitems
      description: Returns a list of your invoice items. Invoice items are returned
        sorted by creation date, with the most recently created invoice items appearing
        first.
      operationId: getInvoiceitems
      x-api-path-slug: invoiceitems-get
      parameters:
      - in: query
        name: created
      - in: query
        name: customer
        description: The identifier of the customer whose invoice items to return
      - in: query
        name: ending_before
        description: A cursor for use in pagination
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: query
        name: limit
        description: A limit on the number of objects to be returned
      - in: query
        name: starting_after
        description: A cursor for use in pagination
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
      tags:
      - Invoiceitems
    post:
      summary: Add Invoiceitems
      description: "Adds an arbitrary charge or credit to the customer\u2019s upcoming
        invoice."
      operationId: postInvoiceitems
      x-api-path-slug: invoiceitems-post
      parameters:
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
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
      tags:
      - Invoiceitems
  /invoiceitems/{invoiceitem}:
    delete:
      summary: Delete Invoiceitems Invoiceitem
      description: "Removes an invoice item from the upcoming invoice. Removing an
        invoice item is only possible before the invoice it\u2019s attached to is
        closed."
      operationId: deleteInvoiceitemsInvoiceitem
      x-api-path-slug: invoiceitemsinvoiceitem-delete
      parameters:
      - in: path
        name: invoiceitem
        description: The identifier of the invoice item to be deleted
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
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
      tags:
      - Invoiceitems
      - Invoiceitem
    get:
      summary: Get Invoiceitems Invoiceitem
      description: Retrieves the invoice item with the given ID.
      operationId: getInvoiceitemsInvoiceitem
      x-api-path-slug: invoiceitemsinvoiceitem-get
      parameters:
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: path
        name: invoiceitem
        description: The ID of the desired invoice item
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
      tags:
      - Invoiceitems
      - Invoiceitem
    post:
      summary: Add Invoiceitems Invoiceitem
      description: "Updates the amount or description of an invoice item on an upcoming
        invoice. Updating an invoice item is only possible before the invoice it\u2019s
        attached to is closed."
      operationId: postInvoiceitemsInvoiceitem
      x-api-path-slug: invoiceitemsinvoiceitem-post
      parameters:
      - in: path
        name: invoiceitem
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
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
      tags:
      - Invoiceitems
      - Invoiceitem
  /subscription_items:
    get:
      summary: Get Subscription Items
      description: Returns a list of your subscription items for a given subscription.
      operationId: getSubscriptionItems
      x-api-path-slug: subscription-items-get
      parameters:
      - in: query
        name: ending_before
        description: A cursor for use in pagination
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: query
        name: limit
        description: A limit on the number of objects to be returned
      - in: query
        name: starting_after
        description: A cursor for use in pagination
      - in: query
        name: subscription
        description: The ID of the subscription whose items will be retrieved
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
      tags:
      - Subscription
      - Items
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