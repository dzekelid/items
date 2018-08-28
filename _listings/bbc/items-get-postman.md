{
  "info": {
    "name": "BBC Nitro Look inside programmes to find segments: chapters, tracks and more",
    "_postman_id": "dddd040e-ebec-4b65-9972-f5a1ecac2743",
    "description": "Look inside programmes to find segments: chapters, tracks and more",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Items",
      "item": [
        {
          "id": "3f5a9ad4-f869-48af-95cb-32051acd19a0",
          "name": "listItems",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/items?authority=%7B%7D&id=%7B%7D&id_type=%7B%7D&item_type=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&people=%7B%7D&pid=%7B%7D&programme=%7B%7D&q=%7B%7D&segment_event=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Look inside programmes to find segments: chapters, tracks and more"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a0cfc89-1c7c-4695-b451-ab6cf35b923f"
            }
          ]
        }
      ]
    }
  ]
}