swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /folders/{FOLDER_ID}/items:
    get:
      summary: Get Folder???s Items
      description: Retrieves the files and/or folders contained within this folder
        without any other metadata about the folder. Any attribute in the full files
        or folders objects can be passed in with the fields parameter to get specific
        attributes, and only those specific attributes back; otherwise, the mini format
        is returned for each item by default. Multiple attributes can be passed in
        separated by commas e.g. fields=name,created_at. Paginated results can be
        retrieved using the limit and offset parameters.
      operationId: getFolderItems
      x-api-path-slug: foldersfolder-iditems-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FOLDER_ID
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The offset at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Folder
      - ""
      - Items
  /folders/trash/items:
    get:
      summary: Get Trashed Items
      description: Retrieves the files and/or folders that have been moved to the
        trash. Any attribute in the full files or folders objects can be passed in
        with the fields parameter to get specific attributes, and only those specific
        attributes back; otherwise, the mini format is returned for each item by default.
        Multiple attributes can be passed in separated by commas e.g. fields=name,created_at.
        Paginated results can be retrieved using the limit and offset parameters.
      operationId: getTrashedItems
      x-api-path-slug: folderstrashitems-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Trash
      - Items
  /shared_items:
    get:
      summary: Shared Items
      description: |-
        Shared items are any files or folders that are represented by a shared link. Shared items are different from other API resources in that a shared resource doesn???t necessarily have to be in the account of the user accessing it. The actual shared link itself is used along with a normal access token.
        Used to retrieve the metadata about a shared item when only given a shared link. Because of varying permission for shared links, a password may be required to retrieve the shared item. Once the item has been retrieved, you can make API requests against the actual resource /files/{id} or /folders/{id} as long as the shared link and optional password are in the header.
      operationId: getSharedItems
      x-api-path-slug: shared-items-get
      parameters:
      - in: header
        name: BoxApi
        description: 'The usage is BoxApi: shared_link=SHARED_LINK&shared_link_password=SHARED_LINK_PASSWORD'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Shared
      - Items
  /collections/{COLLECTION_ID}/items:
    get:
      summary: Get Collection Items
      description: |-
        Retrieves the files and/or folders contained within this collection. Collection item lists behave a lot like getting a folder???s items.
        Paginated results can be retrieved using the limit and offset parameters.
        Sub-object fields can be requested via the ?fields parameter
      operationId: getCollectionItems
      x-api-path-slug: collectionscollection-iditems-get
      parameters:
      - in: path
        name: COLLECTION_ID
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The offset at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Collections
      - Collection
      - ""
      - Items