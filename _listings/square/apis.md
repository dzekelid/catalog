---
name: Square
x-slug: square
description: Starting with a free credit card reader for the iPhone, iPad, and Android
  devices, Square Reader allows anyone to accept credit cards anywhere, anytime, for
  a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square Register
  serves as a full point-of-sale system for businesses to accept payments, manage
  items, and share menu and location information. Square Wallet, available in the
  US, is the most seamless way to pay, enabling individuals to pay at their favorite
  local businesses, discover new ones nearby, explore menu listings, and store receipts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Catalog
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Post V2 Catalog Batch Delete
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/batch-delete
  tags: Catalog,Batch-delete
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchdelete-post-openapi.md
- name: Square Connect API Post V2 Catalog Batch Retrieve
  x-api-slug: square-connect-api
  description: |-
    Returns a set of objects based on the provided ID.
    Each [CatalogItem](#type-catalogitem) returned in the set includes all of its
    child information including: all of its
    [CatalogItemVariation](#type-catalogitemvariation) objects, references to
    its [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
    any [CatalogTax](#type-catalogtax) objects that apply to it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/batch-retrieve
  tags: Catalog,Batch-retrieve
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchretrieve-post-openapi.md
- name: Square Connect API Post V2 Catalog Batch Upsert
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/batch-upsert
  tags: Catalog,Batch-upsert
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogbatchupsert-post-openapi.md
- name: Square Connect API Get V2 Catalog Info
  x-api-slug: square-connect-api
  description: |-
    Returns information about the Square Catalog API, such as batch size
    limits for `BatchUpsertCatalogObjects`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/info
  tags: Catalog,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2cataloginfo-get-openapi.md
- name: Square Connect API Get V2 Catalog List
  x-api-slug: square-connect-api
  description: |-
    Returns a list of [CatalogObject](#type-catalogobject)s that includes
    all objects of a set of desired types (for example, all [CatalogItem](#type-catalogitem)
    and [CatalogTax](#type-catalogtax) objects) in the catalog. The types parameter
    is specified as a comma-separated list of valid [CatalogObject](#type-catalogobject) types:
    `ITEM`, `ITEM_VARIATION`, `MODIFIER`, `MODIFIER_LIST`, `CATEGORY`, `DISCOUNT`, `TAX`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/list
  tags: Catalog,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2cataloglist-get-openapi.md
- name: Square Connect API Post V2 Catalog Object
  x-api-slug: square-connect-api
  description: Creates or updates the target [CatalogObject](#type-catalogobject).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/object
  tags: Catalog,Object
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobject-post-openapi.md
- name: Square Connect API Delete V2 Catalog Object Object
  x-api-slug: square-connect-api
  description: |-
    Deletes a single [CatalogObject](#type-catalogobject) based on the
    provided ID and returns the set of successfully deleted IDs in the response.
    Deletion is a cascading event such that all children of the targeted object
    are also deleted. For example, deleting a [CatalogItem](#type-catalogitem)
    will also delete all of its
    [CatalogItemVariation](#type-catalogitemvariation) children.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/object/{object_id}
  tags: Catalog,Object,Object
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobjectobject-id-delete-openapi.md
- name: Square Connect API Get V2 Catalog Object Object
  x-api-slug: square-connect-api
  description: |-
    Returns a single [CatalogItem](#type-catalogitem) as a
    [CatalogObject](#type-catalogobject) based on the provided ID. The returned
    object includes all of the relevant [CatalogItem](#type-catalogitem)
    information including: [CatalogItemVariation](#type-catalogitemvariation)
    children, references to its
    [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
    any [CatalogTax](#type-catalogtax) objects that apply to it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/object/{object_id}
  tags: Catalog,Object,Object
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogobjectobject-id-get-openapi.md
- name: Square Connect API Post V2 Catalog Search
  x-api-slug: square-connect-api
  description: |-
    Queries the targeted catalog using a variety of query types:
    [CatalogQuerySortedAttribute](#type-catalogquerysortedattribute),
    [CatalogQueryExact](#type-catalogqueryexact),
    [CatalogQueryRange](#type-catalogqueryrange),
    [CatalogQueryText](#type-catalogquerytext),
    [CatalogQueryItemsForTax](#type-catalogqueryitemsfortax), and
    [CatalogQueryItemsForModifierList](#type-catalogqueryitemsformodifierlist).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/search
  tags: Catalog,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogsearch-post-openapi.md
- name: Square Connect API Post V2 Catalog Update Item Modifier Lists
  x-api-slug: square-connect-api
  description: |-
    Updates the [CatalogModifierList](#type-catalogmodifierlist) objects
    that apply to the targeted [CatalogItem](#type-catalogitem) without having
    to perform an upsert on the entire item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/update-item-modifier-lists
  tags: Catalog,Update-item-modifier-lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogupdateitemmodifierlists-post-openapi.md
- name: Square Connect API Post V2 Catalog Update Item Taxes
  x-api-slug: square-connect-api
  description: |-
    Updates the [CatalogTax](#type-catalogtax) objects that apply to the
    targeted [CatalogItem](#type-catalogitem) without having to perform an
    upsert on the entire item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/catalog/update-item-taxes
  tags: Catalog,Update-item-taxes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/v2catalogupdateitemtaxes-post-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Starting with a free credit card reader for the iPhone, iPad, and Android
    devices, Square Reader allows anyone to accept credit cards anywhere, anytime,
    for a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square
    Register serves as a full point-of-sale system for businesses to accept payments,
    manage items, and share menu and location information. Square Wallet, available
    in the US, is the most seamless way to pay, enabling individuals to pay at their
    favorite local businesses, discover new ones nearby, explore menu listings, and
    store receipts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1/
  tags: Catalog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/catalog/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---