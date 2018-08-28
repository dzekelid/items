---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Delete contacts from a contact list
  description: Deletes contacts from a contact list. List the contact ids in request
    to delete multiple contacts with one request.
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