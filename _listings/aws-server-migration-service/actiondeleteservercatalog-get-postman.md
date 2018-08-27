{
  "info": {
    "name": "AWS Server Migration Service API Delete Server Catalog",
    "_postman_id": "82909679-cb51-4a4c-a054-a5b74af86cba",
    "description": "The delete-server-catalog API clears all servers from your server catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Server Catalog",
      "item": [
        {
          "id": "37b7536e-ecff-4833-bdee-60d97d526dfc",
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
              "id": "bc1d18c7-a443-4789-90ec-b54b55a132bd"
            }
          ]
        }
      ]
    }
  ]
}