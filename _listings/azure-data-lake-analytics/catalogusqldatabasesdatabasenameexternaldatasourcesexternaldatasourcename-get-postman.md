{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog Get External Data Source",
    "_postman_id": "02733506-720b-4748-a21e-1b80536d766d",
    "description": "Retrieves the specified external data source from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog external data source",
      "item": [
        {
          "id": "43768872-34d0-42b1-890f-8c26fce925c8",
          "name": "Catalog_GetExternalDataSource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/externaldatasources/:externalDataSourceName"
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
                  "id": "externalDataSourceName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified external data source from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a54355a-85cf-4f7c-b2d7-dbac429f9d42"
            }
          ]
        }
      ]
    }
  ]
}