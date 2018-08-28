---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Move A Drive Item
  description: Move a DriveItem To move a DriveItem to a new parent item, your app
    requests to update the parentReference of the DriveItem to move. This is a special
    case of the Update method. Your app can combine moving an item to a new container
    and updating other properties of the item into a single request.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shares/{sharingIdOrUrl}:
    get:
      summary: Accessing Shared Drive Items
      description: Accessing shared DriveItems Access a shared DriveItem or a collection
        of shared items by using a shareId or sharing URL.
      operationId: AccessingSharedDriveItems
      x-api-path-slug: sharessharingidorurl-get
      parameters:
      - in: path
        name: sharingIdOrUrl
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accessing
      - Shared
      - Drive
      - Items
  /me/drive/items/{item-id}/createLink:
    post:
      summary: Create A Sharing Link For A Drive Item
      description: Create a sharing link for a DriveItem You can use createLink action
        to share a DriveItem via a sharing link.
      operationId: CreateASharingLinkForADriveItem
      x-api-path-slug: medriveitemsitemidcreatelink-post
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - CreateSharing
      - LinkA
      - Drive
      - Item
  /me/drive/root:/{item-path}:/createLink:
    post:
      summary: Create A Sharing Link For A Drive Item
      description: Create a sharing link for a DriveItem You can use createLink action
        to share a DriveItem via a sharing link.
      operationId: CreateASharingLinkForADriveItem
      x-api-path-slug: medriverootitempathcreatelink-post
      parameters:
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - CreateSharing
      - LinkA
      - Drive
      - Item
  /groups/{group-id}/drive/items/{item-id}/createLink:
    post:
      summary: Create A Sharing Link For A Drive Item
      description: Create a sharing link for a DriveItem You can use createLink action
        to share a DriveItem via a sharing link.
      operationId: CreateASharingLinkForADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidcreatelink-post
      parameters:
      - in: path
        name: group-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - CreateSharing
      - LinkA
      - Drive
      - Item
  /drives/{drive-id}/items/{item-id}/createLink:
    post:
      summary: Create A Sharing Link For A Drive Item
      description: Create a sharing link for a DriveItem You can use createLink action
        to share a DriveItem via a sharing link.
      operationId: CreateASharingLinkForADriveItem
      x-api-path-slug: drivesdriveiditemsitemidcreatelink-post
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - CreateSharing
      - LinkA
      - Drive
      - Item
  /me/drive/root:/{item-path}:/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: medriverootitempathcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /me/drive/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: medriveitemsitemidcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /drives/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: drivesitemsitemidcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /groups/{group-id}/drive/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidcontent-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /me/drive/items/{item-id}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: medriveitemsitemid-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: medriveitemsitemid-patch
      parameters:
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /me/drive/root:/{item-path}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: medriverootitempath-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: medriverootitempath-patch
      parameters:
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /drives/{drive-id}/items/{item-id}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: drivesdriveiditemsitemid-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: drivesdriveiditemsitemid-patch
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /groups/{group-id}/drive/items/{item-id}:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemid-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: groupsgroupiddriveitemsitemid-patch
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /me/drive/root/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriverootchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/items/{item-id}/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriveitemsitemidchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/root:/{item-path}:/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriverootitempathchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /drives/{drive-id}/items/{item-id}/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: drivesdriveiditemsitemidchildren-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: medriveitemsitemidpermissions-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /me/drive/root:/{path}:/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: medriverootpathpermissions-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /drives/{drive-id}/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: drivesdriveiditemsitemidpermissions-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /groups/{group-id}/drive/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidpermissions-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /me/drive/root:/{item-path}:/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriverootitempaththumbnails-get
      parameters:
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /me/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /groups/{group-id}/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /groups/{group-id}/drive/{item-id}:
    patch:
      summary: Move A Drive Item
      description: Move a DriveItem To move a DriveItem to a new parent item, your
        app requests to update the parentReference of the DriveItem to move. This
        is a special case of the Update method. Your app can combine moving an item
        to a new container and updating other properties of the item into a single
        request.
      operationId: MoveADriveItem
      x-api-path-slug: groupsgroupiddriveitemid-patch
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - MoveDrive
      - Item
  /me/drive/items/{parent-id}:/{filename}:/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriveitemsparentidfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /me/drive/root:/{parent-path}/{filename}:/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriverootparentpathfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /me/drive/items/{parent-id}/children/{filename}/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriveitemsparentidchildrenfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /groups/{id}/drive/items/{parent-id}/children/{filename}/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: groupsiddriveitemsparentidchildrenfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /workbook/names/add:
    post:
      summary: Add Named Item
      description: Add Named Item Adds a new name to the collection of the given scope
        using the user's locale for the formula.
      operationId: AddNamedItem
      x-api-path-slug: workbooknamesadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer {code}
      responses:
        200:
          description: OK
      tags:
      - Named
      - Item
  /workbook/worksheets({id|name})/names/add:
    post:
      summary: Add Named Item
      description: Add Named Item Adds a new name to the collection of the given scope
        using the user's locale for the formula.
      operationId: AddNamedItem
      x-api-path-slug: workbookworksheetsidnamenamesadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer {code}
      - in: path
        name: id|name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Named
      - Item
  /workbook/names(&lt;name&gt;):
    get:
      summary: Get Named Item
      description: Get NamedItem Retrieve the properties and relationships of nameditem
        object.
      operationId: GetNamedItem
      x-api-path-slug: workbooknamesltnamegt-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Named
      - Item
  /workbook/names:
    get:
      summary: List Named Item Collection
      description: List NamedItemCollection Retrieve a list of nameditem objects.
      operationId: ListNamedItemCollection
      x-api-path-slug: workbooknames-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Named
      - Item
      - Collection
  /workbook/names(&lt;name&gt;)/Range:
    post:
      summary: Named Item Range
      description: 'NamedItem: Range Returns the range object that is associated with
        the name. Throws an exception if the named item''s type is not a range.'
      operationId: NamedItem:Range
      x-api-path-slug: workbooknamesltnamegtrange-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Named
      - Item
      - Range
  /workbook/names(&lt;name&gt;)/range/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbooknamesltnamegtrangeformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/range(&lt;address&gt;)/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegtrangeltaddressgtformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/range/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtrangeformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/tables(&lt;id|name&gt;)/columns/ItemAt:
    post:
      summary: Table Column Collection Item At
      description: 'TableColumnCollection: ItemAt Gets a column based on its position
        in the collection.'
      operationId: TableColumnCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtcolumnsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns/ItemAt:
    post:
      summary: Table Column Collection Item At
      description: 'TableColumnCollection: ItemAt Gets a column based on its position
        in the collection.'
      operationId: TableColumnCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumnsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
      - Item
      - At
  /workbook/tables(&lt;id|name&gt;)/rows/ItemAt:
    post:
      summary: Table Row Collection Item At
      description: 'TableRowCollection: ItemAt Gets a row based on its position in
        the collection.'
      operationId: TableRowCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtrowsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/rows/ItemAt:
    post:
      summary: Table Row Collection Item At
      description: 'TableRowCollection: ItemAt Gets a row based on its position in
        the collection.'
      operationId: TableRowCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtrowsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
      - Item
      - At
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