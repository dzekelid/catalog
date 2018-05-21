{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog List Tables By Database",
    "_postman_id": "104c7ca5-380d-46eb-b23d-50a38aed20cf",
    "description": "Retrieves the list of all tables in a database from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog table database",
      "item": [
        {
          "id": "04069037-9762-4f1d-9915-4bf6ff1d6577",
          "name": "Catalog_ListTablesByDatabase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/tables"
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
            "description": "Retrieves the list of all tables in a database from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1677835-0465-4b7a-a665-13d9cc3d095c"
            }
          ]
        }
      ]
    }
  ]
}