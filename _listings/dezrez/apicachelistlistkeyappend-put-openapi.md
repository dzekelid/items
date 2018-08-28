---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Adds {itemToAppend} to the tail of an existing list, or creates a
    new list with the object in it.
  version: 1.0.0
  description: Adds {itemtoappend} to the tail of an existing list, or creates a new
    list with the object in it..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/ledgerentriescsv:
    post:
      summary: Get ledger items formatted for export csv
      description: Get ledger items formatted for export csv.
      operationId: AccountingExport_ExportLedgerEntriesCsvBydataContract
      x-api-path-slug: apiaccountingexportsledgerentriescsv-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ledger
      - Items
      - Formattedexport
      - Csv
  /api/cache/List/{listKey}/Pop:
    get:
      summary: Pops an items from the list head.
      description: Pops an items from the list head..
      operationId: Cache_PopFromListHeadBylistKey
      x-api-path-slug: apicachelistlistkeypop-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pops
      - Items
      - From
      - List
      - Head
  /api/invoice/raisecreditnote:
    post:
      summary: Raise a credit note against invoice items on an invoice
      description: Raise a credit note against invoice items on an invoice.
      operationId: Invoice_RaiseCreditNoteBycreditNoteDataContract
      x-api-path-slug: apiinvoiceraisecreditnote-post
      parameters:
      - in: body
        name: creditNoteDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Raise
      - Credit
      - Note
      - Against
      - Invoice
      - Items
      - "On"
      - Invoice
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
  /api/list/activesearches/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateActiveSearchCsvBycommandDataContract
      x-api-path-slug: apilistactivesearchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertyfinancial/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateFinancialPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertyfinancialcsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertynewbusiness/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GenerateNewBusinessPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertynewbusinesscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/posting/uncleared:
    post:
      summary: Get uncleared items in accounting system
      description: Get uncleared items in accounting system.
      operationId: Posting_GetUnclearedItemsByunclearedItemsDataContract
      x-api-path-slug: apipostinguncleared-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: unclearedItemsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Uncleared
      - Items
      - In
      - Accounting
      - System
  /api/receipt/paymentitem:
    get:
      summary: Get saved payment items
      description: Get saved payment items.
      operationId: Receipt_GetpaymentItems
      x-api-path-slug: apireceiptpaymentitem-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Payment
      - Items
    put:
      summary: Process payment items
      description: Process payment items.
      operationId: Receipt_ProcessPaymentItems
      x-api-path-slug: apireceiptpaymentitem-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Process
      - Payment
      - Items
    post:
      summary: Saves a payment item to be processed
      description: Saves a payment item to be processed.
      operationId: Receipt_SavePaymentItemByrecordPaymentDataContract
      x-api-path-slug: apireceiptpaymentitem-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Payment
      - Item
      - To
      - Be
      - Processed
    delete:
      summary: Delete a payment item
      description: Delete a payment item.
      operationId: Receipt_DeletePaymentItemByid
      x-api-path-slug: apireceiptpaymentitem-delete
      parameters:
      - in: query
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Item
  /api/reconcile/items:
    post:
      summary: Get all items eligible for reconcile
      description: Get all items eligible for reconcile.
      operationId: Reconcile_GetReconcileItemsByreconcileDataContract
      x-api-path-slug: apireconcileitems-post
      parameters:
      - in: body
        name: reconcileDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Items
      - Eligiblereconcile
  /api/cache/{itemKey}:
    delete:
      summary: Deletes the item stored at {itemKey}
      description: Deletes the item stored at {itemkey}.
      operationId: Cache_DeleteItemByitemKey
      x-api-path-slug: apicacheitemkey-delete
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Item
      - Stored
      - At
      - ItemKey
    get:
      summary: Retrieves an object stored in the cache system by its {itemKey}
      description: Retrieves an object stored in the cache system by its {itemkey}.
      operationId: Cache_GetObjectByitemKey
      x-api-path-slug: apicacheitemkey-get
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Object
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ItemKey
  /api/cache/List/{listKey}/Item:
    delete:
      summary: Removes a given item from the list.
      description: Removes a given item from the list..
      operationId: Cache_RemoveItemFromListByitemToRemoveBylistKey
      x-api-path-slug: apicachelistlistkeyitem-delete
      parameters:
      - in: body
        name: itemToRemove
        description: The item to remove
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Given
      - Item
      - From
      - List
  /api/coreplatformstate/{stateItemReference}:
    delete:
      summary: Clears a state item.
      description: Clears a state item..
      operationId: CorePlatformState_ClearStateItemBystateItemReference
      x-api-path-slug: apicoreplatformstatestateitemreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: stateItemReference
        description: The state item reference
      responses:
        200:
          description: OK
      tags:
      - Clears
      - State
      - Item
  /api/documentgeneration/bulkpropertyownercommunication:
    post:
      summary: "Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
        will ignore the target type set, as the document could only ever find the
        vendor as the contact item, so it always defaults\r\nto a target type of vendor/owner"
      description: "Generates a bulk communication pack out to multiple vendors of
        properties.\r\nthis will ignore the target type set, as the document could
        only ever find the vendor as the contact item, so it always defaults\r\nto
        a target type of vendor/owner."
      operationId: DocumentGeneration_BulkPropertyVendorCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkpropertyownercommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Vendors
      - Of
      - Properties
      - This
      - Will
      - Ignore
      - Target
      - Type
      - Set
      - ""
      - As
      - Document
      - Could
      - Only
      - Ever
      - Find
      - Vendor
      - As
      - Contact
      - Item
      - ""
      - So
      - It
      - Always
      - "Defaults\r\nTo"
      - Target
      - Type
      - Of
      - Vendor
      - Owner
  /api/inboundlead/checkformatchinggroups:
    get:
      summary: Check for Matching groups for the given leads based on contact item
        values i.e. Emails and Phones.
      description: Check for matching groups for the given leads based on contact
        item values i.e. emails and phones..
      operationId: InboundLead_CheckForMatchingGroupsByleadIdBypageSizeBypageNumber
      x-api-path-slug: apiinboundleadcheckformatchinggroups-get
      parameters:
      - in: query
        name: leadId
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - CheckMatching
      - Groupsthe
      - Given
      - Leads
      - Based
      - "On"
      - Contact
      - Item
      - Values
      - I
      - E
      - ""
      - Emails
      - Phones
  /api/invoice/savereceiptlistitem:
    post:
      summary: Save receipt list item
      description: Save receipt list item.
      operationId: Invoice_SaveReceiptListItemBydataContract
      x-api-path-slug: apiinvoicesavereceiptlistitem-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Receipt
      - List
      - Item
  /api/invoice/removereceiptallocation:
    delete:
      summary: Remove a receipt list item allocation
      description: Remove a receipt list item allocation.
      operationId: Invoice_RemoveSavedReceiptItemAllocationByreceiptItemIdByinvoiceIdByallocationId
      x-api-path-slug: apiinvoiceremovereceiptallocation-delete
      parameters:
      - in: query
        name: allocationId
      - in: query
        name: invoiceId
      - in: query
        name: receiptItemId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Receipt
      - List
      - Item
      - Ocation
  /api/progressionchain/{id}/additem:
    post:
      summary: Add item to sales progression chain
      description: Add item to sales progression chain.
      operationId: ProgressionChain_AddItemToChainByidBydataContract
      x-api-path-slug: apiprogressionchainidadditem-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Progression Role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Item
      - To
      - Sales
      - Progression
      - Chain
  /api/progressionchain/{id}/updateitem:
    put:
      summary: Update item in sales progression chain
      description: Update item in sales progression chain.
      operationId: ProgressionChain_UpdateChainItemByidBydataContract
      x-api-path-slug: apiprogressionchainidupdateitem-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Progression Role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Item
      - In
      - Sales
      - Progression
      - Chain
  /api/invoice/processreceiptlistitems:
    put:
      summary: Process receipt list items for a specifici negotiator.
      description: Process receipt list items for a specifici negotiator..
      operationId: Invoice_ProcessReceiptListItemsBynegotiatorId
      x-api-path-slug: apiinvoiceprocessreceiptlistitems-put
      parameters:
      - in: query
        name: negotiatorId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Process
      - Receipt
      - List
      - Itemsa
      - Specifici
      - Negotiator
  /api/people/unsubscribe/{id}:
    get:
      summary: Get All contact items for a person, but obscure the details
      description: Get all contact items for a person, but obscure the details.
      operationId: People_ObscuredContactItemsByid
      x-api-path-slug: apipeopleunsubscribeid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Itemsa
      - Person
      - ""
      - But
      - Obscure
      - Details
    post:
      summary: Unsubscribe/Subscribe All contact items for a person
      description: Unsubscribe/subscribe all contact items for a person.
      operationId: People_UnsubscibedContactItemsByidByitems
      x-api-path-slug: apipeopleunsubscribeid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: items
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
      - Subscribe
      - ""
      - Contact
      - Itemsa
      - Person
  /api/posting/{accountId}/uncleared:
    post:
      summary: Get uncleared items for account/ledger
      description: Get uncleared items for account/ledger.
      operationId: Posting_GetAccountUnclearedItemsByaccountIdByunclearedItemsDataContract
      x-api-path-slug: apipostingaccountiduncleared-post
      parameters:
      - in: path
        name: accountId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: unclearedItemsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Uncleared
      - Itemsaccount
      - Ledger
  /api/cache/List/{listKey}/Append:
    put:
      summary: Adds {itemToAppend} to the tail of an existing list, or creates a new
        list with the object in it.
      description: Adds {itemtoappend} to the tail of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_AppendToListByitemToAppendBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyappend-put
      parameters:
      - in: body
        name: itemToAppend
        description: The item to append
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToAppend
      - To
      - Tail
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/List/{listKey}/Prepend:
    put:
      summary: Adds {itemToPrepend} to the head of an existing list, or creates a
        new list with the object in it.
      description: Adds {itemtoprepend} to the head of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_PrependToListByitemToPrependBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyprepend-put
      parameters:
      - in: body
        name: itemToPrepend
        description: The item to prepend
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToPrepend
      - To
      - Head
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/people/{id}/addcontactitem:
    post:
      summary: Add a ContactItem to a Person
      description: Add a contactitem to a person.
      operationId: People_AddContactItemByidBycontactItemSaveCommandDataContract
      x-api-path-slug: apipeopleidaddcontactitem-post
      parameters:
      - in: body
        name: contactItemSaveCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - ContactItem
      - To
      - Person
  /api/people/{id}/removecontactitem/{contactItemid}:
    put:
      summary: Remove a ContactItem from a Person
      description: Remove a contactitem from a person.
      operationId: People_RemoveContactItemByidBycontactItemid
      x-api-path-slug: apipeopleidremovecontactitemcontactitemid-put
      parameters:
      - in: path
        name: contactItemid
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - ContactItem
      - From
      - Person
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