{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog Get Schema",
    "_postman_id": "223d277a-98be-471f-8b22-26d6a785713a",
    "description": "Retrieves the specified schema from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog schema",
      "item": [
        {
          "id": "a1b163ef-de18-4e4c-83e0-9d287abca7e8",
          "name": "Catalog_GetSchema",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/schemas/:schemaName"
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
                },
                {
                  "id": "schemaName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified schema from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a31592ab-8c08-4c2f-bc1e-279e94c27924"
            }
          ]
        }
      ]
    }
  ]
}