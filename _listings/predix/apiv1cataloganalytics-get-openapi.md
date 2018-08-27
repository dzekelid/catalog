---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Framework Get all analytic catalog entries.
  version: 1.0.0
  description: Returns all analytic catalog entries as specified by page and sort
    criteria.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/catalog/analytics:
    get:
      summary: Get all analytic catalog entries.
      description: Returns all analytic catalog entries as specified by page and sort
        criteria.
      operationId: retrieveAll
      x-api-path-slug: apiv1cataloganalytics-get
      parameters:
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      - in: query
        name: taxonomyPath
        description: 'taxonomy path : taxonomyPath'
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entries
    post:
      summary: Create an analytic catalog entry.
      description: Creates the analytic catalog entry with a generated id.
      operationId: createAnalyticCatalogEntry
      x-api-path-slug: apiv1cataloganalytics-post
      parameters:
      - in: body
        name: body
        description: analytic catalog entry
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/analytics/versions:
    get:
      summary: Get all versions of the analytic catalog entry with the given name.
      description: Returns all versions of the analytic catalog entry with the given
        name.
      operationId: retrieveByName
      x-api-path-slug: apiv1cataloganalyticsversions-get
      parameters:
      - in: query
        name: name
        description: analytic name
      responses:
        200:
          description: OK
      tags:
      - Versions
      - Of
      - Analytic
      - Catalog
      - Entry
      - Given
      - Name
  /api/v1/catalog/analytics/{id}:
    get:
      summary: Get an analytic catalog entry by id.
      description: Returns the analytic catalog entry with the given id.
      operationId: retrieveAnalyticCatalogEntryById
      x-api-path-slug: apiv1cataloganalyticsid-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
    put:
      summary: Update an analytic catalog entry by id.
      description: The analytic catalog entry with the given id will be updated.
      operationId: updateAnalyticCatalogEntry
      x-api-path-slug: apiv1cataloganalyticsid-put
      parameters:
      - in: body
        name: body
        description: analytic catalog entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
    delete:
      summary: Delete an analytic catalog entry by id.
      description: Deletes the analytic catalog entry with the given id.
      operationId: deleteAnalyticCatalogEntryById
      x-api-path-slug: apiv1cataloganalyticsid-delete
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
  /api/v1/catalog/analytics/{id}/artifacts:
    get:
      summary: Get the descriptive information of the artifacts corresponding to an
        analytic catalog entry.
      description: 'Returns the description information (type, description, etc.)
        for all artifacts associated with the given analytic catalog entry id. Note:
        it does not return the artifact file contents; use the download APIs to obtain
        an artifact file. An error is returned if the supplied analytic catalog entry
        id does not exist.'
      operationId: retrieveArtifactsByCatalogEntryId
      x-api-path-slug: apiv1cataloganalyticsidartifacts-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Descriptive
      - Information
      - Of
      - Artifacts
      - Corresponding
      - To
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/analytics/{id}/deployment:
    post:
      summary: Deploy an analytic with an optional deployment configuration by analytic
        catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment with an optional deployment configuration, responds with
        the request id (generated for the request), and the current request status.  The
        force deploy usually takes longer than the standard timeout, so the calling
        process should use the returned request id to monitor the request status and
        to retrieve the deployment results.
      operationId: deployAnalytic
      x-api-path-slug: apiv1cataloganalyticsiddeployment-post
      parameters:
      - in: body
        name: body
        description: deployment configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Deploy
      - Analytic
      - Optional
      - Deployment
      - Configuration
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/analytics/{id}/execution:
    post:
      summary: Execute an analytic by analytic catalog entry id.
      description: This operation executes the specified analytic and responds with
        the result produced by analytic.
      operationId: executeAnalytic
      x-api-path-slug: apiv1cataloganalyticsidexecution-post
      parameters:
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      - in: query
        name: inputId
        description: test artifact id
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Analytic
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/analytics/{id}/validation:
    post:
      summary: Validate an analytic by analytic catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment, runs the analytic and responds with the validation request
        id (generated for the request), and the current request status.  The force
        deploy usually takes longer than the standard timeout, so the calling process
        should use the returned validation request id to monitor the request status
        and to retrieve the validation results.
      operationId: validateAnalytic
      x-api-path-slug: apiv1cataloganalyticsidvalidation-post
      parameters:
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      - in: query
        name: inputId
        description: test artifact id
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Analytic
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/artifacts:
    post:
      summary: Upload an artifact and attach it to an analytic catalog entry.
      description: Upload a single artifact file in a multipart MIME structure and
        attach it to an analytic catalog entry. The multipart MIME structure must
        have the catalog entry id tagged as 'catalogEntryId',  the file contents tagged
        as 'file',  the artifact type tagged as 'type', and  a description (under
        1024 characters) tagged as 'description'. Artifact types can be any string.  Artifacts
        with the type 'executable' must contain the executable for the analytic.   An
        analytic can only have 1 artifact labelled as 'executable'(See the documentation
        for more information regarding these files.)
      operationId: uploadAnalyticArtifact
      x-api-path-slug: apiv1catalogartifacts-post
      parameters:
      - in: formData
        name: catalogEntryId
        description: (Required) analytic catalog entry id
      - in: formData
        name: description
        description: artifact description
      - in: formData
        name: file
        description: (Required) artifact file
      - in: formData
        name: type
        description: (Required) artifact type
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Artifact
      - Attach
      - It
      - To
      - Analytic
      - Catalog
      - Entry
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