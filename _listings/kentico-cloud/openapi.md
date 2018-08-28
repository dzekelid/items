swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
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
  /items:
    get:
      summary: List content items
      description: Retrieve a dynamically paginated list of content items.
      operationId: ItemsGet
      x-api-path-slug: items-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Items
    post:
      summary: Add a content item
      description: |-
        Create a new content item based on a specific content type. Content items do NOT contain any content themselves, but serve as wrappers for individual language variants.

        See <https://developer.kenticocloud.com/v1/reference#content-management-api-add-item> for details about adding content to a specific language variant.

        If you are importing content from a different system and want to use the same identifiers for your content as in the previous system, you can use the `external_id` body attribute to set a custom identifier for the new content item.
      operationId: ItemsPost
      x-api-path-slug: items-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
  /:
    get:
      summary: Getting items by localized URL slug
      description: "Get a *Home* content item whose URL slug in Spanish is *inicio*
        by using the following parameters:\n\n* `language=es-ES` \u2013 specifies
        the codename of the requested language.\n* `system.type=home` \u2013 filters
        content items by their content type.\n* `elements.url_pattern=inicio` \u2013
        filters content items by a value of a specific content element.\n\nSee [Getting
        items by localized URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug)
        for more details."
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Ting
      - Items
      - By
      - Localized
      - URL
      - Slug
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5:
    get:
      summary: View a content item by ID
      description: Retrieve metadata information about a content item specified by
        its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Get
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - ID
    put:
      summary: Update a content item by ID
      description: Update an existing content item specified by its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Put
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - ID
    delete:
      summary: Delete a content item by ID
      description: Delete a content item specified by its internal ID. Note that deleting
        a content item deletes all of its language variants as well.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Delete2
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - ID
  /items/codename/on_roasts:
    get:
      summary: View a content item by codename
      description: Retrieve metadata information about a content item specified by
        its codename.
      operationId: ItemsCodenameOnRoastsGet
      x-api-path-slug: itemscodenameon-roasts-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - Codename
    put:
      summary: Update a content item by codename
      description: Update an existing content item specified by its codename.
      operationId: ItemsCodenameOnRoastsPut
      x-api-path-slug: itemscodenameon-roasts-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - Codename
    delete:
      summary: Delete a content item by codename
      description: |-
        Delete a content item specified by its codename.

        Note that deleting a content item deletes all of its language variants as well.
      operationId: ItemsCodenameOnRoastsDelete
      x-api-path-slug: itemscodenameon-roasts-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - Codename
  /items/external-id/ext-cafe-brno-59713:
    put:
      summary: Creating a content item
      description: "One of the ways to import content to your project is to send a
        PUT request to the `<cmApiUrl>/items/external-id/<your item ID>` endpoint.\r\n\r\nIn
        the body of the request, specify these properties:\r\n\r\n* `name` \u2013
        string with a display name of the new content item.\r\n* `type` \u2013 reference
        to a content type.\r\n* (Optional) `sitemap_locations` \u2013 array of references
        to sitemap locations.\r\n\r\nSee <https://developer.kenticocloud.com/docs/importing-to-kentico-cloud#section-1-creating-a-content-item>
        for more details."
      operationId: ItemsExternalIdExtCafeBrno59713Put
      x-api-path-slug: itemsexternalidextcafebrno59713-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Creating
      - Content
      - Item
  /items/external-id/59713:
    get:
      summary: View a content Item by external ID
      description: Retrieve metadata information about a content item specified by
        its external ID.
      operationId: ItemsExternalId59713Get
      x-api-path-slug: itemsexternalid59713-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - External
      - ID
    put:
      summary: Update a content item by external ID
      description: "Add a new content item or update an existing content item specified
        by its external ID.\r\n\r\n**Note:** If no content item with the specified
        external ID exists in the project, the system will try to create one. For
        existing content items, the API updates the content item's name and sitemap
        locations.\r\nYou can also specify the external ID when [adding content items](https://developer.kenticocloud.com/v1/reference#content-management-api-add-item)
        via the POST method."
      operationId: ItemsExternalId59713Put
      x-api-path-slug: itemsexternalid59713-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - External
      - ID