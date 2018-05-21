{
  "info": {
    "name": "Azure Data Lake Analytics API Catalog List Table Statistics By Database",
    "_postman_id": "17e0ebf8-5ea3-4339-94f7-fe21b934794a",
    "description": "Retrieves the list of all statistics in a database from the Data Lake Analytics catalog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "catalog table statistic database",
      "item": [
        {
          "id": "0db67c45-e6e3-4e4c-ad19-ab3c7904fe0a",
          "name": "Catalog_ListTableStatisticsByDatabase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/statistics"
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
            "description": "Retrieves the list of all statistics in a database from the Data Lake Analytics catalog"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41ee5966-c571-46c9-8dd6-eb0886ff41fc"
            }
          ]
        }
      ]
    }
  ]
}