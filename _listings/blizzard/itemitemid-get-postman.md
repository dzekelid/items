{
  "info": {
    "name": "World of Warcraft Get Item Itemid",
    "_postman_id": "197d6892-6a28-459e-853c-402dd2cf9f1e",
    "description": "Provides detailed item information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Character",
      "item": [
        {
          "id": "169245fa-d593-4e43-b24a-8443d03310c8",
          "name": "getCharacterRealmCharactername",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "character/:realm/:characterName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "characterName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single character at a time through an HTTP GET request to a URL describing the character profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the character's realm, name, level, last modified timestamp, thumbnail, race id, achievement points value, gender id and class id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8168f827-42b1-4147-87ad-e471a501b090"
            }
          ]
        }
      ]
    },
    {
      "name": "Guild",
      "item": [
        {
          "id": "04c7daf3-00d2-4567-8edc-39cc82c0abfa",
          "name": "getGuildRealmGuildname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "guild/:realm/:guildName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "guildName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single guild at a time through an HTTP GET request to a url describing the guild profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the guild's name, level, faction and achievement points."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29673ea4-dd51-4987-b2da-d593ce70e02b"
            }
          ]
        }
      ]
    },
    {
      "name": "Realm",
      "item": [
        {
          "id": "ef01558d-7b13-4192-883b-6af3f142c559",
          "name": "getRealmStatus",
          "request": {
            "url": "http://us.battle.net/api/wow/realm/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves realms status information. This information is limited to whether or not the realm is up, the type and state of the realm and the current population."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f974eb36-bd59-47ca-b41c-8d0a983c38d5"
            }
          ]
        }
      ]
    },
    {
      "name": "Auction",
      "item": [
        {
          "id": "a89d5a2f-220c-4e97-9e1a-3e452a0b9abc",
          "name": "getAuctionDataRealm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "auction/data/:realm"
              ],
              "variable": [
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a per-realm list of recently generated auction house data dumps. The current auctions data is represented as JSON structures containing auction data for the tree auctions houses available on each realm."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e66a8b0-1e34-46a1-9b99-673b8d0d24fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "76789269-f894-4de9-9662-fe71731bb59c",
          "name": "getItemItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "item/:itemId"
              ],
              "variable": [
                {
                  "id": "itemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides detailed item information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90dea4ab-767f-4554-a704-b71f138b3157"
            }
          ]
        }
      ]
    }
  ]
}