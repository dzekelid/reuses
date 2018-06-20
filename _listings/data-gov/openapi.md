---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/org_reuses/:
    get:
      summary: Get Me Org Reuses
      description: List all reuses related to me and my organizations
      operationId: getMeOrgReuses
      x-api-path-slug: meorg-reuses-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Reuses
  /me/reuses/:
    get:
      summary: Get Me Reuses
      description: List all my reuses (including private ones)
      operationId: getMeReuses
      x-api-path-slug: mereuses-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Reuses
  /organizations/{org}/reuses/:
    get:
      summary: Get Organizations Org Reuses
      description: List organization reuses (including private ones when member)
      operationId: getOrganizationsOrgReuses
      x-api-path-slug: organizationsorgreuses-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Reuses
  /reuses/:
    get:
      summary: Get Reuses
      description: Get Reuses
      operationId: getReuses
      x-api-path-slug: reuses-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: dataset
      - in: query
        name: datasets
      - in: query
        name: extra
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: featured
      - in: query
        name: followers
      - in: query
        name: organization
      - in: query
        name: owner
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      - in: query
        name: tag
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Reuses
    post:
      summary: Add Reuses
      description: Create a new object
      operationId: postReuses
      x-api-path-slug: reuses-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reuses
  /reuses/badges/:
    get:
      summary: Get Reuses Badges
      description: List all available reuse badges and their labels
      operationId: getReusesBadges
      x-api-path-slug: reusesbadges-get
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Badges
  /reuses/suggest/:
    get:
      summary: Get Reuses Suggest
      description: Suggest reuses
      operationId: getReusesSuggest
      x-api-path-slug: reusessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Suggest
  /reuses/types/:
    get:
      summary: Get Reuses Types
      description: List all reuse types
      operationId: getReusesTypes
      x-api-path-slug: reusestypes-get
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Types
  /reuses/{id}/followers/:
    delete:
      summary: Delete Reuses  Followers
      description: Unfollow an object given its ID
      operationId: deleteReusesFollowers
      x-api-path-slug: reusesidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
    get:
      summary: Get Reuses  Followers
      description: List all followers for a given object
      operationId: getReusesFollowers
      x-api-path-slug: reusesidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
    post:
      summary: Add Reuses  Followers
      description: Follow an object given its ID
      operationId: postReusesFollowers
      x-api-path-slug: reusesidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
  /reuses/{reuse}/:
    delete:
      summary: Delete Reuses Reuse
      description: Delete a given reuse
      operationId: deleteReusesReuse
      x-api-path-slug: reusesreuse-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    get:
      summary: Get Reuses Reuse
      description: Fetch a given reuse
      operationId: getReusesReuse
      x-api-path-slug: reusesreuse-get
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    put:
      summary: Put Reuses Reuse
      description: Update a given reuse
      operationId: putReusesReuse
      x-api-path-slug: reusesreuse-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
  /reuses/{reuse}/badges/:
    post:
      summary: Add Reuses Reuse Badges
      description: Create a new badge for a given reuse
      operationId: postReusesReuseBadges
      x-api-path-slug: reusesreusebadges-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
  /reuses/{reuse}/badges/{badge_kind}/:
    delete:
      summary: Delete Reuses Reuse Badges Badge Kind
      description: Delete a badge for a given reuse
      operationId: deleteReusesReuseBadgesBadgeKind
      x-api-path-slug: reusesreusebadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
      - Badge
      - Kind
  /reuses/{reuse}/datasets/:
    post:
      summary: Add Reuses Reuse Datasets
      description: Add a dataset to a given reuse
      operationId: postReusesReuseDatasets
      x-api-path-slug: reusesreusedatasets-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Datasets
  /reuses/{reuse}/featured/:
    delete:
      summary: Delete Reuses Reuse Featured
      description: Unmark a reuse as featured
      operationId: deleteReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
    post:
      summary: Add Reuses Reuse Featured
      description: Mark a reuse as featured
      operationId: postReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-post
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
  /reuses/{reuse}/image:
    post:
      summary: Add Reuses Reuse Image
      description: Upload a new reuse image
      operationId: postReusesReuseImage
      x-api-path-slug: reusesreuseimage-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Image
  /site/home/reuses/:
    get:
      summary: Get Site Home Reuses
      description: List homepage featured reuses
      operationId: getSiteHomeReuses
      x-api-path-slug: sitehomereuses-get
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
    put:
      summary: Put Site Home Reuses
      description: Set the homepage reuses editorial selection
      operationId: putSiteHomeReuses
      x-api-path-slug: sitehomereuses-put
      parameters:
      - in: body
        name: payload
        description: Reuse IDs to put in homepage
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
---