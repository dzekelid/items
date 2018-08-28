swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  item/{id}/:
    get:
      summary: Get Item
      description: Get items.
      operationId: getItem
      x-api-path-slug: itemid-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: query
        name: format
        description: The format of the returned content item data
      - in: query
        name: id
        description: The GUID of a content item (not case-sensitive)
      responses:
        200:
          description: OK
      tags:
      - Item
  item/{mediaType}/{id}/{rendition}:
    get:
      summary: Get Item Mediatype Rendition
      description: Pulls item media
      operationId: getItemMediatypeRendition
      x-api-path-slug: itemmediatypeidrendition-get
      parameters:
      - in: query
        name: apiKey
        description: API key
      - in: query
        name: filename
        description: The filename for the downloaded content item rendition, in the
          format
      - in: query
        name: id
        description: The GUID of a content item (not case-sensitive)
      - in: query
        name: mediaType
        description: The content media type
      - in: query
        name: rendition
        description: The content item rendition
      responses:
        200:
          description: OK
      tags:
      - Item
      - Mediatype
      - Rendition