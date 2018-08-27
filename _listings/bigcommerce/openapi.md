swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
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