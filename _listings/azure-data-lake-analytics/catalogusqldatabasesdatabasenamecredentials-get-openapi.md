---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Catalog List Credentials
  description: Retrieves the list of credentials from the Data Lake Analytics catalog.
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
  /catalog/usql/databases/{databaseName}/credentials/{credentialName}:
    put:
      summary: Catalog Create Credential
      description: Creates the specified credential for use with external data sources
        in the specified database.
      operationId: Catalog_CreateCredential
      x-api-path-slug: catalogusqldatabasesdatabasenamecredentialscredentialname-put
      parameters:
      - in: path
        name: credentialName
        description: The name of the credential
      - in: path
        name: databaseName
        description: The name of the database in which to create the credential
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters required to create the credential (name and password)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Catalog Credential
    patch:
      summary: Catalog Update Credential
      description: Modifies the specified credential for use with external data sources
        in the specified database
      operationId: Catalog_UpdateCredential
      x-api-path-slug: catalogusqldatabasesdatabasenamecredentialscredentialname-patch
      parameters:
      - in: path
        name: credentialName
        description: The name of the credential
      - in: path
        name: databaseName
        description: The name of the database containing the credential
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters required to modify the credential (name and password)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Catalog Credential
    get:
      summary: Catalog Get Credential
      description: Retrieves the specified credential from the Data Lake Analytics
        catalog.
      operationId: Catalog_GetCredential
      x-api-path-slug: catalogusqldatabasesdatabasenamecredentialscredentialname-get
      parameters:
      - in: path
        name: credentialName
        description: The name of the credential
      - in: path
        name: databaseName
        description: The name of the database containing the schema
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Credential
    post:
      summary: Catalog Delete Credential
      description: Deletes the specified credential in the specified database
      operationId: Catalog_DeleteCredential
      x-api-path-slug: catalogusqldatabasesdatabasenamecredentialscredentialname-post
      parameters:
      - in: query
        name: cascade
        description: Indicates if the delete should be a cascading delete (which deletes
          all resources dependent on the credential as well as the credential) or
          not
      - in: path
        name: credentialName
        description: The name of the credential to delete
      - in: path
        name: databaseName
        description: The name of the database containing the credential
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters to delete a credential if the current user is
          not the account owner
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Catalog Credential
  /catalog/usql/databases/{databaseName}/credentials:
    get:
      summary: Catalog List Credentials
      description: Retrieves the list of credentials from the Data Lake Analytics
        catalog.
      operationId: Catalog_ListCredentials
      x-api-path-slug: catalogusqldatabasesdatabasenamecredentials-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the schema
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Credentials
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