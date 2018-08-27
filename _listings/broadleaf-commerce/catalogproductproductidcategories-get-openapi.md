---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Catalog Product Categories
  description: Get catalog product categories.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/categories:
    get:
      summary: Get Catalog Categories
      description: Get catalog categories.
      operationId: getCatalogCategories
      x-api-path-slug: catalogcategories-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: name
        description: name
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Categories
  /catalog/category:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategory
      x-api-path-slug: catalogcategory-get
      parameters:
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: searchParameter
        description: searchParameter
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategoryCategory
      x-api-path-slug: catalogcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}/activeSubcategories:
    get:
      summary: Get Catalog Category Active Subcategories
      description: Get catalog category active subcategories.
      operationId: getCatalogCategoryCategoryActivesubcategories
      x-api-path-slug: catalogcategorycategoryidactivesubcategories-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Active
      - Subcategories
  /catalog/category/{categoryId}/attributes:
    get:
      summary: Get Catalog Category Attributes
      description: Get catalog category attributes.
      operationId: getCatalogCategoryCategoryAttributes
      x-api-path-slug: catalogcategorycategoryidattributes-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Attributes
  /catalog/category/{categoryId}/categories:
    get:
      summary: Get Catalog Category Categories
      description: Get catalog category categories.
      operationId: getCatalogCategoryCategoryCategories
      x-api-path-slug: catalogcategorycategoryidcategories-get
      parameters:
      - in: query
        name: active
        description: active
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Categories
  /catalog/category/{id}/media:
    get:
      summary: Get Catalog Category Media
      description: Get catalog category media.
      operationId: getCatalogCategoryMedia
      x-api-path-slug: catalogcategoryidmedia-get
      parameters:
      - in: path
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Media
  /catalog/product/{id}:
    get:
      summary: Get Catalog Product
      description: Get catalog product.
      operationId: getCatalogProduct
      x-api-path-slug: catalogproductid-get
      parameters:
      - in: path
        name: id
        description: id
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
  /catalog/product/{productId}/attributes:
    get:
      summary: Get Catalog Product Attributes
      description: Get catalog product attributes.
      operationId: getCatalogProductProductAttributes
      x-api-path-slug: catalogproductproductidattributes-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Attributes
  /catalog/product/{productId}/categories:
    get:
      summary: Get Catalog Product Categories
      description: Get catalog product categories.
      operationId: getCatalogProductProductCategories
      x-api-path-slug: catalogproductproductidcategories-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Categories
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