---
name: Square
x-slug: square
description: Square helps millions of sellers run their business- from secure credit
  card processing to point of sale solutions. Get paid faster with Square and sign
  up today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
x-kinRank: "9"
x-alexaRank: "2436"
tags: Catalog
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API BatchDeleteCatalogObjects
  x-api-slug: square-connect-api
  description: |-
    Deletes a set of [CatalogItem](#type-catalogitem)s based on the
    provided list of target IDs and returns a set of successfully deleted IDs in
    the response. Deletion is a cascading event such that all children of the
    targeted object are also deleted. For example, deleting a CatalogItem will
    also delete all of its [CatalogItemVariation](#type-catalogitemvariation)
    children.

    `BatchDeleteCatalogObjects` succeeds even if only a portion of the targeted
    IDs can be deleted. The response will only include IDs that were
    actually deleted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/batch-delete
  tags: BatchCatalogObjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchdelete-post-openapi.md
- name: Square Connect API BatchRetrieveCatalogObjects
  x-api-slug: square-connect-api
  description: |-
    Returns a set of objects based on the provided ID.
    Each [CatalogItem](#type-catalogitem) returned in the set includes all of its
    child information including: all of its
    [CatalogItemVariation](#type-catalogitemvariation) objects, references to
    its [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
    any [CatalogTax](#type-catalogtax) objects that apply to it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/batch-retrieve
  tags: BatchRetrieveCatalogObjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchretrieve-post-openapi.md
- name: Square Connect API BatchUpsertCatalogObjects
  x-api-slug: square-connect-api
  description: |-
    Creates or updates up to 10,000 target objects based on the provided
    list of objects. The target objects are grouped into batches and each batch is
    inserted/updated in an all-or-nothing manner. If an object within a batch is
    malformed in some way, or violates a database constraint, the entire batch
    containing that item will be disregarded. However, other batches in the same
    request may still succeed. Each batch may contain up to 1,000 objects, and
    batches will be processed in order as long as the total object count for the
    request (items, variations, modifier lists, discounts, and taxes) is no more
    than 10,000.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/batch-upsert
  tags: BatchUpsertCatalogObjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchupsert-post-openapi.md
- name: Square Connect API CatalogInfo
  x-api-slug: square-connect-api
  description: |-
    Returns information about the Square Catalog API, such as batch size
    limits for `BatchUpsertCatalogObjects`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/info
  tags: CatalogInfo
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2cataloginfo-get-openapi.md
- name: Square Connect API ListCatalog
  x-api-slug: square-connect-api
  description: |-
    Returns a list of [CatalogObject](#type-catalogobject)s that includes
    all objects of a set of desired types (for example, all [CatalogItem](#type-catalogitem)
    and [CatalogTax](#type-catalogtax) objects) in the catalog. The types parameter
    is specified as a comma-separated list of valid [CatalogObject](#type-catalogobject) types:
    `ITEM`, `ITEM_VARIATION`, `MODIFIER`, `MODIFIER_LIST`, `CATEGORY`, `DISCOUNT`, `TAX`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/list
  tags: ListCatalog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2cataloglist-get-openapi.md
- name: Square Connect API UpsertCatalogObject
  x-api-slug: square-connect-api
  description: Creates or updates the target [CatalogObject](#type-catalogobject).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/object
  tags: UpsertCatalogObject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobject-post-openapi.md
- name: Square Connect API DeleteCatalogObject
  x-api-slug: square-connect-api
  description: |-
    Deletes a single [CatalogObject](#type-catalogobject) based on the
    provided ID and returns the set of successfully deleted IDs in the response.
    Deletion is a cascading event such that all children of the targeted object
    are also deleted. For example, deleting a [CatalogItem](#type-catalogitem)
    will also delete all of its
    [CatalogItemVariation](#type-catalogitemvariation) children.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/object/{object_id}
  tags: CatalogObject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobjectobject-id-delete-openapi.md
- name: Square Connect API RetrieveCatalogObject
  x-api-slug: square-connect-api
  description: |-
    Returns a single [CatalogItem](#type-catalogitem) as a
    [CatalogObject](#type-catalogobject) based on the provided ID. The returned
    object includes all of the relevant [CatalogItem](#type-catalogitem)
    information including: [CatalogItemVariation](#type-catalogitemvariation)
    children, references to its
    [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
    any [CatalogTax](#type-catalogtax) objects that apply to it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/object/{object_id}
  tags: RetrieveCatalogObject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobjectobject-id-get-openapi.md
- name: Square Connect API SearchCatalogObjects
  x-api-slug: square-connect-api
  description: |-
    Queries the targeted catalog using a variety of query types
    ([CatalogQuerySortedAttribute](#type-catalogquerysortedattribute),
    ([CatalogQueryExact](#type-catalogqueryexact),
    ([CatalogQueryRange](#type-catalogqueryrange),
    ([CatalogQueryText](#type-catalogquerytext),
    ([CatalogQueryItemsForTax](#type-catalogqueryitemsfortax),
    ([CatalogQueryItemsForModifierList](#type-catalogqueryitemsformodifierlist)).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/search
  tags: SearchCatalogObjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogsearch-post-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Square helps millions of sellers run their business- from secure credit
    card processing to point of sale solutions. Get paid faster with Square and sign
    up today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com//
  tags: Catalog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-crunchbase
  url: https://crunchbase.com/organization/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-email
  url: press@squareup.com
- type: x-email
  url: security@squareup.com
- type: x-email
  url: lawenforcement@squareup.com
- type: x-email
  url: redemption@squareup.com
- type: x-email
  url: privacy@squareup.com
- type: x-email
  url: community@squareup.com
- type: x-email
  url: noreply@messaging.squareup.com
- type: x-email
  url: ir@squareup.com
- type: x-email
  url: takedowns@squareup.com
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: http://squareup.com
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---