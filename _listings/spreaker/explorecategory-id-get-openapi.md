---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Explore Category Items
  version: v1
  description: 'This API returns information and items of a specific category. The
    response contains two properties at root level:'
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /explore/{category_id}:
    get:
      summary: Explore Category Items
      description: 'This API returns information and items of a specific category.
        The response contains two properties at root level:'
      operationId: getExploreCategory
      x-api-path-slug: explorecategory-id-get
      parameters:
      - in: query
        name: explore_category
        description: contains category information, the exact same information exported
          by /explore/categories API
      - in: query
        name: items
        description: contains a sorted list of shows or episodes, depending on the
          category type (type 1 and 3 contain episodes, type 2 contains shows)
      responses:
        200:
          description: OK
      tags:
      - Explore
      - Category
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