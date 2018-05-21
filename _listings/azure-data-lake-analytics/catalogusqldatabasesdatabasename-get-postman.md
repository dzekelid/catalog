{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog Get Database",
    "_postman_id": "4e003d71-585f-4195-b771-5a9851e6f768",
    "description": "Retrieves the specified database from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog database",
      "item": [
        {
          "id": "a4ee6e9d-5138-4c4c-b32c-cff6faf853ff",
          "name": "Catalog_GetDatabase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "databaseName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified database from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7d233c3-a4c6-4590-8dc1-51c18a2879c8"
            }
          ]
        }
      ]
    }
  ]
}