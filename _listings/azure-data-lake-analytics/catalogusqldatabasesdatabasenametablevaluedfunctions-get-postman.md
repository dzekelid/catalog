{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog List Table Valued Functions By Database",
    "_postman_id": "6d0640c2-5026-45a8-ac72-e1074da0131d",
    "description": "Retrieves the list of all table valued functions in a database from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog table valued function database",
      "item": [
        {
          "id": "1a6df511-7a9b-4429-a9bd-ae1522bdf87b",
          "name": "Catalog_ListTableValuedFunctionsByDatabase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/tablevaluedfunctions"
              ],
              "query": [
                {
                  "key": "$count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$orderby",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$select",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Retrieves the list of all table valued functions in a database from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b82aab19-f676-407b-a43e-be982d0913eb"
            }
          ]
        }
      ]
    }
  ]
}