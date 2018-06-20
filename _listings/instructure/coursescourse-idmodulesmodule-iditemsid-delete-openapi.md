---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Delete module item
  description: Delete module item.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/modules/module_id/items:
    get:
      summary: List module items
      description: List module items.
      operationId: list-module-items
      x-api-path-slug: coursescourse-idmodulesmodule-iditems-get
      parameters:
      - in: query
        name: include[]
        description: If included, will return additional details specific to the contentnassociated
          with each item
      - in: query
        name: search_term
        description: The partial title of the items to match and return
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
    post:
      summary: Create a module item
      description: Create a module item.
      operationId: create-a-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditems-post
      parameters:
      - in: query
        name: module_item[completion_requirement][min_score]
        description: Minimum score required to complete
      - in: query
        name: module_item[completion_requirement][type]
        description: Completion requirement for this module item
      - in: query
        name: module_item[content_id]
        description: The id of the content to link to the module item
      - in: query
        name: module_item[external_url]
        description: External url that the item points to
      - in: query
        name: module_item[indent]
        description: 0-based indent level; module items may be indented to show a
          hierarchy
      - in: query
        name: module_item[new_tab]
        description: Whether the external tool opens in a new tab
      - in: query
        name: module_item[page_url]
        description: Suffix for the linked wiki page (e
      - in: query
        name: module_item[position]
        description: The position of this item in the module (1-based)
      - in: query
        name: module_item[title]
        description: The name of the module item and associated content
      - in: query
        name: module_item[type]
        description: 'The type of content linked to the itemnn        n        n          Allowed
          values: File, Page, Discussion, Assignment, Quiz, SubHeader, ExternalUrl,
          ExternalTool'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
  /courses/{course_id}/modules/module_id/items/{id}:
    delete:
      summary: Delete module item
      description: Delete module item.
      operationId: delete-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
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