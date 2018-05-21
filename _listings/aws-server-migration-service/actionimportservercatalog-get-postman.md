{
  "info": {
    "name": "AWS Server Migration Service API Import Server Catalog",
    "_postman_id": "ac4e7670-c3cb-48a8-9a73-fbb9184e1c53",
    "description": "The import-server-catalog API is used to gather the complete list of on-premises servers on your premises.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Server Catalog",
      "item": [
        {
          "id": "5d1ac45e-18fd-425b-92cd-342fb7fdcecb",
          "name": "deleteServerCatalog",
          "request": {
            "url": "http://example.com/api/?Action=DeleteServerCatalog",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The delete-server-catalog API clears all servers from your server catalog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f169b6d-13dd-4e0a-b3d1-79fae31b62ef"
            }
          ]
        },
        {
          "id": "d124dc07-32e8-4de0-8f95-e9168dab02e2",
          "name": "importServerCatalog",
          "request": {
            "url": "http://example.com/api/?Action=ImportServerCatalog",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The import-server-catalog API is used to gather the complete list of on-premises servers on your premises."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82f27ae4-8c28-4d27-985e-65d1b40d6ee4"
            }
          ]
        }
      ]
    }
  ]
}