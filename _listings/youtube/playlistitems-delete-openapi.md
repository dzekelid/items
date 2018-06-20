---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Delete Play List Items
  description: Deletes a playlist item.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlistItems:
    delete:
      summary: Delete Play List Items
      description: Deletes a playlist item.
      operationId: deletePlaylistitems
      x-api-path-slug: playlistitems-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube playlist item ID for the
          playlist item that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
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