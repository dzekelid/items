---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
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
    put:
      summary: Put Play List Items
      description: Modifies a playlist item. For example, you could update the item's
        position in the playlist.
      operationId: putPlaylistitems
      x-api-path-slug: playlistitems-put
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
  /groupItems:
    delete:
      summary: Delete Groupitems
      description: Removes an item from a group.
      operationId: deleteGroupitems
      x-api-path-slug: groupitems-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube group item ID for the
          group that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
    get:
      summary: Get Groupitems
      description: Returns a collection of group items that match the API request
        parameters.
      operationId: getGroupitems
      x-api-path-slug: groupitems-get
      parameters:
      - in: query
        name: groupId
        description: The id parameter specifies the unique ID of the group for which
          you want to retrieve group items
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
    post:
      summary: Add Groupitems
      description: Creates a group item.
      operationId: postGroupitems
      x-api-path-slug: groupitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
---