---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Reuses
  description: Get Reuses
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