---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Catalog Delete All Secrets
  description: Deletes all secrets in the specified database. This is deprecated and
    will be removed in the next release. In the future, please only drop individual
    credentials using DeleteCredential
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/usql/databases/{databaseName}/secrets/{secretName}:
    put:
      summary: Catalog Create Secret
      description: Creates the specified secret for use with external data sources
        in the specified database. This is deprecated and will be removed in the next
        release. Please use CreateCredential instead.
      operationId: Catalog_CreateSecret
      x-api-path-slug: catalogusqldatabasesdatabasenamesecretssecretname-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database in which to create the secret
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters required to create the secret (name and password)
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: secretName
        description: The name of the secret
      responses:
        200:
          description: OK
      tags:
      - Catalog Secret
    patch:
      summary: Catalog Update Secret
      description: Modifies the specified secret for use with external data sources
        in the specified database. This is deprecated and will be removed in the next
        release. Please use UpdateCredential instead.
      operationId: Catalog_UpdateSecret
      x-api-path-slug: catalogusqldatabasesdatabasenamesecretssecretname-patch
      parameters:
      - in: path
        name: databaseName
        description: The name of the database containing the secret
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters required to modify the secret (name and password)
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: secretName
        description: The name of the secret
      responses:
        200:
          description: OK
      tags:
      - Catalog Secret
    get:
      summary: Catalog Get Secret
      description: Gets the specified secret in the specified database. This is deprecated
        and will be removed in the next release. Please use GetCredential instead.
      operationId: Catalog_GetSecret
      x-api-path-slug: catalogusqldatabasesdatabasenamesecretssecretname-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database containing the secret
      - in: query
        name: No Name
      - in: path
        name: secretName
        description: The name of the secret to get
      responses:
        200:
          description: OK
      tags:
      - Catalog Secret
    delete:
      summary: Catalog Delete Secret
      description: Deletes the specified secret in the specified database. This is
        deprecated and will be removed in the next release. Please use DeleteCredential
        instead.
      operationId: Catalog_DeleteSecret
      x-api-path-slug: catalogusqldatabasesdatabasenamesecretssecretname-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database containing the secret
      - in: query
        name: No Name
      - in: path
        name: secretName
        description: The name of the secret to delete
      responses:
        200:
          description: OK
      tags:
      - Catalog Secret
  /catalog/usql/databases/{databaseName}/secrets:
    delete:
      summary: Catalog Delete All Secrets
      description: Deletes all secrets in the specified database. This is deprecated
        and will be removed in the next release. In the future, please only drop individual
        credentials using DeleteCredential
      operationId: Catalog_DeleteAllSecrets
      x-api-path-slug: catalogusqldatabasesdatabasenamesecrets-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database containing the secret
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog All Secrets
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---