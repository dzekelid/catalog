---
name: Azure Data Lake Analytics
x-slug: azure-data-lake-analytics
description: The Data Lake analytics service is a new distributed analytics service
  built on Apache YARN that dynamically scales so you can focus on your business goals,
  not on distributed infrastructure. Instead of deploying, configuring and tuning
  hardware, you write queries to transform your data and extract valuable insights.
  The analytics service can handle jobs of any scale instantly by simply setting the
  dial for how much power you need. You only pay for your job when it is running making
  it cost-effective. The analytics service supports Azure Active Directory letting
  you simply manage access and roles, integrated with your on-premises identity system.
  It also includes U-SQL, a language that unifies the benefits of SQL with the expressive
  power of user code. U-SQL&rsquo;s scalable distributed runtime enables you to efficiently
  analyze data in the store and across SQL Servers in Azure, Azure SQL Database and
  Azure SQL Data Warehouse.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
x-kinRank: "10"
x-alexaRank: ""
tags: Catalog
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Data Lake Analytics API Catalog Create Secret
  x-api-slug: azure-data-lake-analytics-api
  description: Creates the specified secret for use with external data sources in
    the specified database. This is deprecated and will be removed in the next release.
    Please use CreateCredential instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/secrets/{secretName}
  tags: Catalog Secret
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamesecretssecretname-put-openapi.md
- name: Azure Data Lake Analytics API Catalog Update Secret
  x-api-slug: azure-data-lake-analytics-api
  description: Modifies the specified secret for use with external data sources in
    the specified database. This is deprecated and will be removed in the next release.
    Please use UpdateCredential instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/secrets/{secretName}
  tags: Catalog Secret
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamesecretssecretname-patch-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Secret
  x-api-slug: azure-data-lake-analytics-api
  description: Gets the specified secret in the specified database. This is deprecated
    and will be removed in the next release. Please use GetCredential instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/secrets/{secretName}
  tags: Catalog Secret
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamesecretssecretname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Delete Secret
  x-api-slug: azure-data-lake-analytics-api
  description: Deletes the specified secret in the specified database. This is deprecated
    and will be removed in the next release. Please use DeleteCredential instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/secrets/{secretName}
  tags: Catalog Secret
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamesecretssecretname-delete-openapi.md
- name: Azure Data Lake Analytics API Catalog Delete All Secrets
  x-api-slug: azure-data-lake-analytics-api
  description: Deletes all secrets in the specified database. This is deprecated and
    will be removed in the next release. In the future, please only drop individual
    credentials using DeleteCredential
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/secrets
  tags: Catalog All Secrets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamesecrets-delete-openapi.md
- name: Azure Data Lake Analytics API Catalog Create Credential
  x-api-slug: azure-data-lake-analytics-api
  description: Creates the specified credential for use with external data sources
    in the specified database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/credentials/{credentialName}
  tags: Catalog Credential
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamecredentialscredentialname-put-openapi.md
- name: Azure Data Lake Analytics API Catalog Update Credential
  x-api-slug: azure-data-lake-analytics-api
  description: Modifies the specified credential for use with external data sources
    in the specified database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/credentials/{credentialName}
  tags: Catalog Credential
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamecredentialscredentialname-patch-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Credential
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified credential from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/credentials/{credentialName}
  tags: Catalog Credential
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamecredentialscredentialname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Delete Credential
  x-api-slug: azure-data-lake-analytics-api
  description: Deletes the specified credential in the specified database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/credentials/{credentialName}
  tags: Catalog Credential
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamecredentialscredentialname-post-openapi.md
- name: Azure Data Lake Analytics API Catalog List Credentials
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of credentials from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/credentials
  tags: Catalog Credentials
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamecredentials-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get External Data Source
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified external data source from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/externaldatasources/{externalDataSourceName}
  tags: Catalog External Data Source
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameexternaldatasourcesexternaldatasourcename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameexternaldatasourcesexternaldatasourcename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List External Data Sources
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of external data sources from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/externaldatasources
  tags: Catalog External Data Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameexternaldatasources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameexternaldatasources-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Procedure
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified procedure from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/procedures/{procedureName}
  tags: Catalog Procedure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanameproceduresprocedurename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Procedures
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of procedures from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/procedures
  tags: Catalog Procedures
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanameprocedures-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Table
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified table from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}
  tags: Catalog Table
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablestablename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Tables
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of tables from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables
  tags: Catalog Tables
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametables-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Statistics By Database And
    Schema
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all table statistics within the specified schema
    from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/statistics
  tags: Catalog Table Statistic Database Schema
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamestatistics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamestatistics-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Table Type
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified table type from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tabletypes/{tableTypeName}
  tags: Catalog Table Type
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametabletypestabletypename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Types
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of table types from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tabletypes
  tags: Catalog Table Types
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametabletypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametabletypes-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Package
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified package from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/packages/{packageName}
  tags: Catalog Package
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamepackagespackagename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Packages
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of packages from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/packages
  tags: Catalog Packages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamepackages-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get View
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified view from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/views/{viewName}
  tags: Catalog View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanameviewsviewname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Views
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of views from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/views
  tags: Catalog Views
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanameviews-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Table Statistic
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified table statistics from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}/statistics/{statisticsName}
  tags: Catalog Table Statistic
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablestablenamestatisticsstatisticsname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Statistics
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of table statistics from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}/statistics
  tags: Catalog Table Statistics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablestablenamestatistics-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Table Partition
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified table partition from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}/partitions/{partitionName}
  tags: Catalog Table Partition
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablestablenamepartitionspartitionname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Partitions
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of table partitions from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}/partitions
  tags: Catalog Table Partitions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablestablenamepartitions-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Types
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of types within the specified database and schema
    from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/types
  tags: Catalog Types
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametypes-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Table Valued Function
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified table valued function from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tablevaluedfunctions/{tableValuedFunctionName}
  tags: Catalog Table Valued Function
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablevaluedfunctionstablevaluedfunctionname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Valued Functions
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of table valued functions from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/tablevaluedfunctions
  tags: Catalog Table Valued Functions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablevaluedfunctions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanametablevaluedfunctions-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Assembly
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified assembly from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/assemblies/{assemblyName}
  tags: Catalog Assembly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameassembliesassemblyname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Assemblies
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of assemblies from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/assemblies
  tags: Catalog Assemblies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameassemblies-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Schema
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified schema from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}
  tags: Catalog Schema
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemaname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemaname-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Schemas
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of schemas from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas
  tags: Catalog Schemas
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemas-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemas-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Statistics By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all statistics in a database from the Data Lake
    Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/statistics
  tags: Catalog Table Statistic Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamestatistics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamestatistics-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Tables By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all tables in a database from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/tables
  tags: Catalog Table Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametables-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Valued Functions By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all table valued functions in a database from
    the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/tablevaluedfunctions
  tags: Catalog Table Valued Function Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametablevaluedfunctions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametablevaluedfunctions-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Views By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all views in a database from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/views
  tags: Catalog View Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameviews-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified database from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}
  tags: Catalog Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Databases
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of databases from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases
  tags: Catalog Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/catalogusqldatabases-get-openapi.md
- name: Azure Data Lake Analytics API
  x-api-slug: azure-data-lake-analytics-api
  description: The Data Lake analytics service is a new distributed analytics service
    built on Apache YARN that dynamically scales so you can focus on your business
    goals, not on distributed infrastructure. Instead of deploying, configuring and
    tuning hardware, you write queries to transform your data and extract valuable
    insights. The analytics service can handle jobs of any scale instantly by simply
    setting the dial for how much power you need. You only pay for your job when it
    is running making it cost-effective. The analytics service supports Azure Active
    Directory letting you simply manage access and roles, integrated with your on-premises
    identity system. It also includes U-SQL, a language that unifies the benefits
    of SQL with the expressive power of user code. U-SQL&rsquo;s scalable distributed
    runtime enables you to efficiently analyze data in the store and across SQL Servers
    in Azure, Azure SQL Database and Azure SQL Data Warehouse.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Catalog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/azure-data-lake-analytics/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/data-lake-analytics/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/data-lake-analytics/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/data-lake-analytics/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/data-lake-analytics/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---