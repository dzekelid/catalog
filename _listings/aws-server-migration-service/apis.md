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
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Server Migration Service API Delete Server Catalog
  x-api-slug: aws-server-migration-service-api
  description: The delete-server-catalog API clears all servers from your server catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
  humanURL: https://aws.amazon.com/server-migration-service/
  baseURL: ://///?Action=DeleteServerCatalog
  tags: Server Catalog
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actiondeleteservercatalog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actiondeleteservercatalog-get-openapi.md
- name: AWS Server Migration Service API Import Server Catalog
  x-api-slug: aws-server-migration-service-api
  description: The import-server-catalog API is used to gather the complete list of
    on-premises servers on your premises.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
  humanURL: https://aws.amazon.com/server-migration-service/
  baseURL: ://///?Action=ImportServerCatalog
  tags: 'Server Catalog '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actionimportservercatalog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/actionimportservercatalog-get-openapi.md
- name: AWS Server Migration Service API
  x-api-slug: aws-server-migration-service-api
  description: AWS Server Migration Service (SMS) is an agentless service which makes
    it easier and faster for you to migrate thousands of on-premises workloads to
    AWS. AWS SMS allows you to automate, schedule, and track incremental replications
    of live server volumes, making it easier for you to coordinate large-scale server
    migrations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AMI.png
  humanURL: https://aws.amazon.com/server-migration-service/
  baseURL: :///
  tags: Catalog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/aws-server-migration-service/openapi.md
x-common:
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