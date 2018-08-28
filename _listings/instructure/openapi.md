swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
    get:
      summary: Show module item
      description: Show module item.
      operationId: show-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-get
      parameters:
      - in: query
        name: include[]
        description: If included, will return additional details specific to the contentnassociated
          with this item
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
      - Id
    put:
      summary: Update a module item
      description: Update a module item.
      operationId: update-a-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-put
      parameters:
      - in: query
        name: module_item[completion_requirement][min_score]
        description: Minimum score required to complete, Required for completion_requirementntype
          &#39;min_score&#39;
      - in: query
        name: module_item[completion_requirement][type]
        description: Completion requirement for this module item
      - in: query
        name: module_item[external_url]
        description: External url that the item points to
      - in: query
        name: module_item[indent]
        description: 0-based indent level; module items may be indented to show a
          hierarchy
      - in: query
        name: module_item[module_id]
        description: Move this item to another module by specifying the target module
          id here
      - in: query
        name: module_item[new_tab]
        description: Whether the external tool opens in a new tab
      - in: query
        name: module_item[position]
        description: The position of this item in the module (1-based)
      - in: query
        name: module_item[published]
        description: Whether the module item is published and visible to students
      - in: query
        name: module_item[title]
        description: The name of the module item
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
  /courses/{course_id}/modules/module_id/items/{id}/done:
    put:
      summary: Mark module item as done/not done
      description: Mark module item as done/not done.
      operationId: mark-module-item-as-donenot-done
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsiddone-put
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
      - Done
  /courses/{course_id}/modules/module_id/items/{id}/mark_read:
    post:
      summary: Mark module item read
      description: Mark module item read.
      operationId: mark-module-item-read
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsidmark-read-post
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
      - Mark
      - Read
  /courses/{course_id}/module_item_sequence:
    get:
      summary: Get module item sequence
      description: Get module item sequence.
      operationId: get-module-item-sequence
      x-api-path-slug: coursescourse-idmodule-item-sequence-get
      parameters:
      - in: query
        name: asset_id
        description: The id of the asset (or the url in the case of a Page)
      - in: query
        name: asset_type
        description: The type of asset to find module sequence information for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Module
      - Item
      - Sequence