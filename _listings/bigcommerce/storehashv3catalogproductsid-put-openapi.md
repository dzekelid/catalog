---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Update a product in the catalog
  description: Updates a single product's information in the catalog
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store-hash}/v3/catalog/products/{id}:
    put:
      summary: Update a product in the catalog
      description: Updates a single product's information in the catalog
      operationId: V3CatalogProductsByStoreHashAndIdPut
      x-api-path-slug: storehashv3catalogproductsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - In
      - Catalog
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