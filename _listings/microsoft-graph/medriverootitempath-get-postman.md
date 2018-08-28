{
  "info": {
    "name": "Microsoft Graph API Get A Drive Item Resource",
    "_postman_id": "13b3bd4f-8940-4847-a271-abe3b515a5e8",
    "description": "Get a DriveItem resource Retrieve the metadata for a DriveItem in a Drive by file system path or ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachment",
      "item": [
        {
          "id": "a9ce37f5-744b-4c1f-b91f-51d97bd4c267",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f8b139b-c871-43b2-99f9-f0971f5622dc"
            }
          ]
        },
        {
          "id": "2f40894c-6539-434b-9486-e026fdaabb96",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12650c3e-939f-4dbd-9356-95e9d55ae073"
            }
          ]
        },
        {
          "id": "c8f9ccfa-e6ff-49c2-bdfd-e61c524666c2",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ab1810a-7441-44f3-ac3c-f84be83a5d54"
            }
          ]
        },
        {
          "id": "43d64428-03bd-4adb-ac47-2c8bf2669a1b",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendar/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74dcd316-49db-40bf-9b5e-5492e1b1764a"
            }
          ]
        },
        {
          "id": "4289b311-8e2b-4ced-92ce-8797ce3b25f5",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f64413fd-6b86-4111-bca3-3fff7ebb04e2"
            }
          ]
        },
        {
          "id": "f84b7776-db3a-4208-bba7-f90e927a16ab",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb1e9f1-2dd7-4bba-a0b2-479eeeb0d5d1"
            }
          ]
        },
        {
          "id": "a60de542-feca-47ac-9eda-32dac111907c",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e850424c-95db-4bf5-86e5-84f91317431c"
            }
          ]
        },
        {
          "id": "4f2712a0-760f-4764-b3e7-4a450c81a7ee",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "388c076c-f2a5-4930-acc1-34dc098a1117"
            }
          ]
        },
        {
          "id": "c724318c-7aa0-4415-a0d1-815ef60bec26",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroup/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c9099ff-235c-42c0-8bb6-cf8f68458427"
            }
          ]
        },
        {
          "id": "f00bd282-21a4-4869-8526-0ff46e3ea5d0",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroup/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3e899cd-880f-42b8-9214-fb0758febcf9"
            }
          ]
        },
        {
          "id": "b998bb87-66a5-4a7a-94ca-524cfde8e80f",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebaf7f54-649a-4ff3-9235-2d5a87f8c240"
            }
          ]
        },
        {
          "id": "f30e0e4e-a9c5-4398-a198-933cc8bf3aed",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3a1a4ec-f759-48f2-a186-52b333e83dbe"
            }
          ]
        },
        {
          "id": "a66aeb18-ee23-437f-8ec7-b6e17f6fe09b",
          "name": "GetAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "111484d2-ad56-463d-80d7-fbf2745c5b7f"
            }
          ]
        },
        {
          "id": "d4e1f5e5-62f7-4954-8c6b-bb9f078e6832",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d67fa0bb-ccf1-464f-9bb3-41a7f157b2e1"
            }
          ]
        },
        {
          "id": "d15f29e1-3e8b-4c0d-b173-633049028ea3",
          "name": "GetAttachment8",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ccb4294-296d-4061-aa25-e34b10a0dbf3"
            }
          ]
        },
        {
          "id": "b7ee23dd-43e0-4fda-b47e-8386398ae882",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "332e3c8b-fbea-44f2-b39f-1e53396f5852"
            }
          ]
        },
        {
          "id": "c4fb58c5-bdea-4d9c-a764-1d67d942efc2",
          "name": "GetAttachment9",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/threads/:id/posts/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e20db82-29a3-401c-90d9-729cab63c5b8"
            }
          ]
        },
        {
          "id": "9e1e3dbb-817d-451c-8f53-41c9c1133441",
          "name": "GetAttachment10",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/conversations/:id/threads/:id/posts/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6ade8a2-f3bb-4606-868e-25473b079c26"
            }
          ]
        },
        {
          "id": "8cba7187-f7b8-43a4-8e05-239ae38e5d28",
          "name": "AddAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da77103a-b9a6-481d-9d2a-569ee7490f19"
            }
          ]
        },
        {
          "id": "d578a77b-dd30-4d25-91c4-200d0ad5fda1",
          "name": "AddAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82f5929a-834b-46a0-8a80-97b45e9be915"
            }
          ]
        },
        {
          "id": "57e9c21a-8cf3-4040-8435-776aafc4de79",
          "name": "AddAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3f84cea-6f00-4529-b0f4-f9948113ccf0"
            }
          ]
        },
        {
          "id": "00a328a1-02b8-4b7e-87ea-ef8456dd3c3a",
          "name": "AddAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71839882-ae1b-4e4f-aac4-583901ee9a33"
            }
          ]
        },
        {
          "id": "63943283-3fc3-4852-a104-31233cfa3749",
          "name": "AddAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df1ba860-a417-44ac-b473-17d4a7926232"
            }
          ]
        },
        {
          "id": "202b397e-97f5-4d39-a99e-1f71f91d3fff",
          "name": "AddAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9ebed1-577b-47b9-9c02-939a1da4a47d"
            }
          ]
        },
        {
          "id": "21cab571-d9aa-46b1-8a8e-74ed4d59276e",
          "name": "AddAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8de2785-d39b-403d-94dd-c9fa7c9dcac4"
            }
          ]
        },
        {
          "id": "e91baf23-ce9e-4fce-92d4-b67dde8e61dc",
          "name": "AddAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcc28c1e-671e-4b8c-bb85-f2c5540fa8d8"
            }
          ]
        },
        {
          "id": "c3912718-e9df-42e3-af19-f559910b330d",
          "name": "AddAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroup/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "806da6b1-e78c-4c74-b40e-1c0066a50a91"
            }
          ]
        },
        {
          "id": "c8e67ec5-4169-4494-a4f9-a76270b1de5c",
          "name": "AddAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroup/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "502d12a4-b310-45fb-94c8-2a26fc835671"
            }
          ]
        },
        {
          "id": "a5ef5a18-0a26-4158-a5ea-4556da1862ac",
          "name": "AddAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroups/:id/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbc398be-14ba-4754-b91a-5cff6c1a3bc1"
            }
          ]
        },
        {
          "id": "c82a5e08-667c-4754-bbd6-54ad3c291f07",
          "name": "AddAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroups/:id/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a54d587d-3beb-4dbc-96a2-59b7e1e88f6d"
            }
          ]
        },
        {
          "id": "095b4351-7163-44f4-86f5-b2973b710ef9",
          "name": "AddAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02004415-53fd-4ef6-aa36-d3ac0b09a395"
            }
          ]
        },
        {
          "id": "f40eb507-15e7-4e21-91dc-0c6d71dcb771",
          "name": "AddAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6640dd21-f027-4ba4-a4ca-bc673fa70255"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b3f93aec-8371-4435-b19e-ba40be2c328b",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/childFolders/:id/.../messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "620e21d0-1d5e-451f-bc29-04d9388ab078"
            }
          ]
        },
        {
          "id": "1b748c57-804d-4e87-b827-0d3e13349533",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/childFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e50df12-4bab-48d8-9473-e932e7dcb6f6"
            }
          ]
        },
        {
          "id": "7e5a646d-23bc-4b9c-afa1-1c44278c9553",
          "name": "ListCalendarView",
          "request": {
            "url": "http://graph.microsoft.com/me/calendar/calendarView?endDateTime=endDateTime&startDateTime=startDateTime",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c67956d-8465-4e8e-8dd4-aef07918b716"
            }
          ]
        },
        {
          "id": "79f5d0d7-78f2-47ee-bf76-f0025e1f7049",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af44bce8-ee99-4cf4-9aa6-5822772baf09"
            }
          ]
        },
        {
          "id": "0f2d993b-ba41-488b-a8ff-226e3c6acdaa",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "107b11fe-ffed-4ed4-86f6-ef1b332e6d41"
            }
          ]
        },
        {
          "id": "cb2b269c-f380-4961-a07b-38a5243a5dcf",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da6a40a3-967c-478d-882f-ba52408dd1cd"
            }
          ]
        },
        {
          "id": "11208707-052e-4ccc-9550-5a05de96ea38",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e74d4ee-36ac-45dd-ba43-4f4984c40ae0"
            }
          ]
        },
        {
          "id": "54a19d95-cf5c-41ba-83e9-803cba2debf8",
          "name": "ListCalendarView1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroup/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1307756-7807-4168-8d6d-6c1ee6ed4de0"
            }
          ]
        },
        {
          "id": "05ed0922-ea7d-405d-8bb8-ae8b9d68b2b4",
          "name": "ListCalendarView1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroup/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8a94746-8ced-421d-8ae1-306222fffebf"
            }
          ]
        },
        {
          "id": "2fcbf6a8-51de-46a4-afe6-1bf7c7835f36",
          "name": "ListCalendarView2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroups/:id/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false