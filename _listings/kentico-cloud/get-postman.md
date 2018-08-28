{
  "info": {
    "name": "Kentico Cloud Getting items by localized URL slug",
    "_postman_id": "197b193c-16ed-4db2-aa62-0e2306eefcfa",
    "description": "Get a *Home* content item whose URL slug in Spanish is *inicio* by using the following parameters:\n\n* `language=es-ES` – specifies the codename of the requested language.\n* `system.type=home` – filters content items by their content type.\n* `elements.url_pattern=inicio` – filters content items by a value of a specific content element.\n\nSee [Getting items by localized URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug) for more details.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ting",
      "item": [
        {
          "id": "d469d0d8-db17-4ff2-ab61-3b60dbbb107c",
          "name": "UnnammedEndpointGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a *Home* content item whose URL slug in Spanish is *inicio* by using the following parameters:\n\n* `language=es-ES` – specifies the codename of the requested language.\n* `system.type=home` – filters content items by their content type.\n* `elements.url_pattern=inicio` – filters content items by a value of a specific content element.\n\nSee [Getting items by localized URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug) for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab3292bf-fcc7-42b3-9f47-b71bbd76b0ad"
            }
          ]
        }
      ]
    }
  ]
}