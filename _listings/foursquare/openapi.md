swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{LIST_ID}/additem:
    post:
      summary: Post Lists Additem
      description: /lists/{LIST_ID}/suggestvenues
      operationId: listslist-idsuggestvenues
      x-api-path-slug: listslist-idadditem-post
      parameters:
      - in: query
        name: itemId
        description: Used in conjuction with listId, the id of an item on that list
          that we wish to copy to this list
      - in: query
        name: listId
        description: Used in conjuction with itemId, the id for a user created or
          followed list as well as one of USER_ID/tips, USER_ID/todos, or USER_ID/dones
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list as well as one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: text
        description: If the target is a user-created list, this will create a public
          tip on the venue
      - in: query
        name: tipId
        description: Used to add a tip to a list
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: A venue to add to the list
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/deleteitem:
    post:
      summary: Post Lists Deleteitem
      description: /lists/{LIST_ID}/additem
      operationId: listslist-idadditem
      x-api-path-slug: listslist-iddeleteitem-post
      parameters:
      - in: query
        name: itemId
        description: Id of the item to delete
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/updateitem:
    post:
      summary: Post Lists Updateitem
      description: /lists/{LIST_ID}/update
      operationId: listslist-idupdate
      x-api-path-slug: listslist-idupdateitem-post
      parameters:
      - in: query
        name: itemId
        description: The id of an item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: photoId
        description: If present and a non-empty value, adds a photo to this item
      - in: query
        name: text
        description: If present creates a public tip on the venue and replaces any
          existing tip on the item
      - in: query
        name: tipId
        description: If present and a non-empty value, adds or replaces a tip on this
          item
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item