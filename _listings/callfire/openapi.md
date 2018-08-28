swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/lists/{id}/items:
    delete:
      summary: Delete contacts from a contact list
      description: Deletes contacts from a contact list. List the contact ids in request
        to delete multiple contacts with one request.
      operationId: removeContactListItems
      x-api-path-slug: contactslistsiditems-delete
      parameters:
      - in: query
        name: contactId
        description: An id of a contact entity in the CallFire system
      - in: path
        name: id
        description: A id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
    get:
      summary: Find contacts in a contact list
      description: Searches for all entries in a contact list with specified id. Returns
        a paged list of contact entries
      operationId: getContactListItems
      x-api-path-slug: contactslistsiditems-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a contact list
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
    post:
      summary: Add contacts to a contact list
      description: 'Adds contacts to a contact list. Available contact sources are:
        list of the contact entities, list of ids of existing contacts in user''s
        account, list of phone numbers in E.164 format (11-digits)'
      operationId: addContactListItems
      x-api-path-slug: contactslistsiditems-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
  /contacts/lists/{id}/items/{contactId}:
    delete:
      summary: Delete a contact from a contact list
      description: Deletes a single contact from a contact list
      operationId: removeContactListItem
      x-api-path-slug: contactslistsiditemscontactid-delete
      parameters:
      - in: path
        name: contactId
        description: An id of a contact
      - in: path
        name: id
        description: An id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
      - ContactId