{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog List Databases",
    "_postman_id": "7ea76f87-192e-462a-9220-4679e76b8a33",
    "description": "Retrieves the list of databases from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog databases",
      "item": [
        {
          "id": "0436d68a-14c2-47b2-8db1-66ac566ae6df",
          "name": "Catalog_ListDatabases",
          "request": {
            "url": "http://example.com/catalog/usql/databases?$count=%7B%7D&$filter=%7B%7D&$orderby=%7B%7D&$select=%7B%7D&$skip=%7B%7D&$top=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of databases from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67765165-de13-422f-897e-969e8bd3c2a0"
            }
          ]
        }
      ]
    }
  ]
}