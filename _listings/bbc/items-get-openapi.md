---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: 'BBC Nitro Look inside programmes to find segments: chapters, tracks and
    more'
  description: 'Look inside programmes to find segments: chapters, tracks and more'
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /items:
    get:
      summary: 'Look inside programmes to find segments: chapters, tracks and more'
      description: 'Look inside programmes to find segments: chapters, tracks and
        more'
      operationId: listItems
      x-api-path-slug: items-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of items that have an ID issued by the given
          authority
      - in: query
        name: id
        description: filter for subset of items having given ID
      - in: query
        name: id_type
        description: filter for subset of items that have given an ID of the given
          type
      - in: query
        name: item_type
        description: filter for specific type(s) of items
      - in: query
        name: mixin
        description: 'Mixins:* contributions: mixin to return information about contributors
          to items* images: mixin to add image information for an item* offset: mixin
          to return programme segment offsets, works in conjunction with programme
          filter* play_event: mixin to return programme segment events, works in conjunction
          with programme or segment_event filters'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for items by partner ID
      - in: query
        name: partner_pid
        description: filter for items by partner PID
      - in: query
        name: people
        description: filter for subset of items that have specified person involved
      - in: query
        name: pid
        description: filter for subset of items matching one of the given PIDs
      - in: query
        name: programme
        description: filter for subset of items that are part of the given programme
      - in: query
        name: q
        description: filter for subset of items matching supplied keyword/phrase (boolean
          operators permitted)
      - in: query
        name: segment_event
        description: filter for item with the given segment_event
      - in: query
        name: sort
        description: 'Sorts:* pid: sort by pid, descending'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
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