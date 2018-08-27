---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Catalog
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Analytics Catalog - Get all analytic catalog entries.
  x-api-slug: apiv1cataloganalytics-get
  description: Returns all analytic catalog entries as specified by page and sort
    criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalytics-get-openapi.md
- name: Analytics Catalog - Create an analytic catalog entry.
  x-api-slug: apiv1cataloganalytics-post
  description: Creates the analytic catalog entry with a generated id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalytics-post-openapi.md
- name: Analytics Catalog - Get all versions of the analytic catalog entry with the
    given name.
  x-api-slug: apiv1cataloganalyticsversions-get
  description: Returns all versions of the analytic catalog entry with the given name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsversions-get-openapi.md
- name: Analytics Catalog - Get an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-get
  description: Returns the analytic catalog entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-get-openapi.md
- name: Analytics Catalog - Update an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-put
  description: The analytic catalog entry with the given id will be updated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-put-openapi.md
- name: Analytics Catalog - Delete an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-delete
  description: Deletes the analytic catalog entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-delete-openapi.md
- name: Analytics Catalog - Get the descriptive information of the artifacts corresponding
    to an analytic catalog entry.
  x-api-slug: apiv1cataloganalyticsidartifacts-get
  description: 'Returns the description information (type, description, etc.) for
    all artifacts associated with the given analytic catalog entry id. Note: it does
    not return the artifact file contents; use the download APIs to obtain an artifact
    file. An error is returned if the supplied analytic catalog entry id does not
    exist.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidartifacts-get-openapi.md
- name: Analytics Catalog - Deploy an analytic with an optional deployment configuration
    by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsiddeployment-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment with an optional deployment configuration, responds with the
    request id (generated for the request), and the current request status.  The force
    deploy usually takes longer than the standard timeout, so the calling process
    should use the returned request id to monitor the request status and to retrieve
    the deployment results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsiddeployment-post-openapi.md
- name: Analytics Catalog - Execute an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidexecution-post
  description: This operation executes the specified analytic and responds with the
    result produced by analytic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidexecution-post-openapi.md
- name: Analytics Catalog - Validate an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidvalidation-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment, runs the analytic and responds with the validation request
    id (generated for the request), and the current request status.  The force deploy
    usually takes longer than the standard timeout, so the calling process should
    use the returned validation request id to monitor the request status and to retrieve
    the validation results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidvalidation-post-openapi.md
- name: Analytics Catalog - Upload an artifact and attach it to an analytic catalog
    entry.
  x-api-slug: apiv1catalogartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an analytic catalog entry. The multipart MIME structure must have the catalog
    entry id tagged as 'catalogEntryId',  the file contents tagged as 'file',  the
    artifact type tagged as 'type', and  a description (under 1024 characters) tagged
    as 'description'. Artifact types can be any string.  Artifacts with the type 'executable'
    must contain the executable for the analytic.   An analytic can only have 1 artifact
    labelled as 'executable'(See the documentation for more information regarding
    these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1catalogartifacts-post-openapi.md
- name: Analytics Framework - Get all analytic catalog entries.
  x-api-slug: apiv1cataloganalytics-get
  description: Returns all analytic catalog entries as specified by page and sort
    criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalytics-get-openapi.md
- name: Analytics Framework - Create an analytic catalog entry.
  x-api-slug: apiv1cataloganalytics-post
  description: Creates the analytic catalog entry with a generated id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalytics-post-openapi.md
- name: Analytics Framework - Get all versions of the analytic catalog entry with
    the given name.
  x-api-slug: apiv1cataloganalyticsversions-get
  description: Returns all versions of the analytic catalog entry with the given name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsversions-get-openapi.md
- name: Analytics Framework - Get an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-get
  description: Returns the analytic catalog entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-get-openapi.md
- name: Analytics Framework - Update an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-put
  description: The analytic catalog entry with the given id will be updated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-put-openapi.md
- name: Analytics Framework - Delete an analytic catalog entry by id.
  x-api-slug: apiv1cataloganalyticsid-delete
  description: Deletes the analytic catalog entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsid-delete-openapi.md
- name: Analytics Framework - Get the descriptive information of the artifacts corresponding
    to an analytic catalog entry.
  x-api-slug: apiv1cataloganalyticsidartifacts-get
  description: 'Returns the description information (type, description, etc.) for
    all artifacts associated with the given analytic catalog entry id. Note: it does
    not return the artifact file contents; use the download APIs to obtain an artifact
    file. An error is returned if the supplied analytic catalog entry id does not
    exist.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidartifacts-get-openapi.md
- name: Analytics Framework - Deploy an analytic with an optional deployment configuration
    by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsiddeployment-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment with an optional deployment configuration, responds with the
    request id (generated for the request), and the current request status.  The force
    deploy usually takes longer than the standard timeout, so the calling process
    should use the returned request id to monitor the request status and to retrieve
    the deployment results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsiddeployment-post-openapi.md
- name: Analytics Framework - Execute an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidexecution-post
  description: This operation executes the specified analytic and responds with the
    result produced by analytic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidexecution-post-openapi.md
- name: Analytics Framework - Validate an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidvalidation-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment, runs the analytic and responds with the validation request
    id (generated for the request), and the current request status.  The force deploy
    usually takes longer than the standard timeout, so the calling process should
    use the returned validation request id to monitor the request status and to retrieve
    the validation results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1cataloganalyticsidvalidation-post-openapi.md
- name: Analytics Framework - Upload an artifact and attach it to an analytic catalog
    entry.
  x-api-slug: apiv1catalogartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an analytic catalog entry. The multipart MIME structure must have the catalog
    entry id tagged as 'catalogEntryId',  the file contents tagged as 'file',  the
    artifact type tagged as 'type', and  a description (under 1024 characters) tagged
    as 'description'. Artifact types can be any string.  Artifacts with the type 'executable'
    must contain the executable for the analytic.   An analytic can only have 1 artifact
    labelled as 'executable'(See the documentation for more information regarding
    these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/apiv1catalogartifacts-post-openapi.md
- name: Event Audit Trail Documentation - Get Catalog
  x-api-slug: v2catalog-get
  description: Get catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://event-audit-trail.run.aws-usw02-pr.ice.predix.io//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/v2catalog-get-openapi.md
- name: Nurego API - Get Catalog
  x-api-slug: v1catalog-get
  description: You can retrieve the service catalog for specific distribution channels,
    segments or customers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://api.nurego.com//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/predix/v1catalog-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---