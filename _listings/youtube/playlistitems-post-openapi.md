---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Play List Items
  description: Adds a resource to a playlist.
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
    get:
      summary: Get Play List Items
      description: Returns a collection of playlist items that match the API request
        parameters. You can retrieve all of the playlist items in a specified playlist
        or retrieve one or more playlist items by their unique IDs.
      operationId: getPlaylistitems
      x-api-path-slug: playlistitems-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of one or more
          unique playlist item IDs
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more playlistItem resource properties that the API response will include
      - in: query
        name: playlistId
        description: The playlistId parameter specifies the unique ID of the playlist
          for which you want to retrieve playlist items
      - in: query
        name: videoId
        description: The videoId parameter specifies that the request should return
          only the playlist items that contain the specified video
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
    post:
      summary: Add Play List Items
      description: Adds a resource to a playlist.
      operationId: postPlaylistitems
      x-api-path-slug: playlistitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
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