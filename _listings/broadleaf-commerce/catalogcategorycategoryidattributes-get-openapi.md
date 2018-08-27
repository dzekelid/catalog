---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Catalog Category Attributes
  description: Get catalog category attributes.
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