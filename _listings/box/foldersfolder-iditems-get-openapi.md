---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Folder???s Items
  description: Retrieves the files and/or folders contained within this folder without
    any other metadata about the folder. Any attribute in the full files or folders
    objects can be passed in with the fields parameter to get specific attributes,
    and only those specific attributes back; otherwise, the mini format is returned
    for each item by default. Multiple attributes can be passed in separated by commas
    e.g. fields=name,created_at. Paginated results can be retrieved using the limit
    and offset parameters.
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