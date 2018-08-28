---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud Getting localized content items
  description: |-
    Get a content item in a specific language variant by using the `language` parameter.

    See [Getting localized content items](https://developer.kenticocloud.com/docs/localization#section-getting-localized-content-items) for more details.
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /975bf280-fd91-488c-994c-2f04416e5ee3/items/on_roasts:
    get:
      summary: Getting localized content items
      description: |-
        Get a content item in a specific language variant by using the `language` parameter.

        See [Getting localized content items](https://developer.kenticocloud.com/docs/localization#section-getting-localized-content-items) for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3ItemsOnRoastsGet3
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3itemson-roasts-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: language
      responses:
        200:
          description: OK
      tags:
      - Ting
      - Localized
      - Content
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