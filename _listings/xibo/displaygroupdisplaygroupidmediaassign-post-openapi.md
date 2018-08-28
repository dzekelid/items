---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Assign one or more Media items to a Display Group
  description: Adds the provided Media to the Display Group
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/media/assign:
    post:
      summary: Assign one or more Media items to a Display Group
      description: Adds the provided Media to the Display Group
      operationId: displayGroupMediaAssign
      x-api-path-slug: displaygroupdisplaygroupidmediaassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: mediaId
        description: The Media Ids to assign
      - in: formData
        name: unassignMediaId
        description: Optional array of Media Id to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - Media
      - Items
      - To
      - Display
      - Group
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