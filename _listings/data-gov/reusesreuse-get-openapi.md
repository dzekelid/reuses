---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Reuses Reuse
  description: Fetch a given reuse
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