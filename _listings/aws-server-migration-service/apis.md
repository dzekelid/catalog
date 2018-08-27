---
name: AWS Server Migration Service
x-slug: aws-server-migration-service
description: AWS Server Migration Service (SMS) is an agentless service which makes
  it easier and faster for you to migrate thousands of on-premises workloads to AWS.
  AWS SMS allows you to automate, schedule, and track incremental replications of
  live server volumes, making it easier for you to coordinate large-scale server migrations.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Catalog
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Server Migration Service API - Delete Server Catalog
  x-api-slug: actiondeleteservercatalog-get
  description: The delete-server-catalog API clears all servers from your server catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
  humanURL: https://aws.amazon.com/server-migration-service/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Databases, Migrations, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actiondeleteservercatalog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actiondeleteservercatalog-get-openapi.md
- name: AWS Server Migration Service API - Import Server Catalog
  x-api-slug: actionimportservercatalog-get
  description: The import-server-catalog API is used to gather the complete list of
    on-premises servers on your premises.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
  humanURL: https://aws.amazon.com/server-migration-service/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Databases, Migrations, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actionimportservercatalog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actionimportservercatalog-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.security.token.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.server.migration.service.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/server-migration-service/latest/userguide/cli_workflow.html
- type: x-documentation
  url: http://docs.aws.amazon.com/ServerMigration/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/server-migration-service/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/server-migration-service/getting-started/
- type: x-partners
  url: https://aws.amazon.com/server-migration-service/partners/
- type: x-pricing
  url: https://aws.amazon.com/server-migration-service/pricing/
- type: x-website
  url: https://aws.amazon.com/server-migration-service/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---