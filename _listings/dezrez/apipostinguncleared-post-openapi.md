---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get uncleared items in accounting system
  version: 1.0.0
  description: Get uncleared items in accounting system.
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