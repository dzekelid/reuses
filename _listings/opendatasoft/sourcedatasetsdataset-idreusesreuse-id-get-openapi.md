---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Datasets Dataset Reuses Reuse
  description: Retrieve a single reuse based on its ID.
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{source}/datasets/{dataset_id}/reuses:
    get:
      summary: Get Source Datasets Dataset Reuses
      description: Get list of reuses
      operationId: getDatasetReuses
      x-api-path-slug: sourcedatasetsdataset-idreuses-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Reuses
  /{source}/datasets/{dataset_id}/reuses/{reuse_id}:
    get:
      summary: Get Source Datasets Dataset Reuses Reuse
      description: Retrieve a single reuse based on its ID.
      operationId: getDatasetReuse
      x-api-path-slug: sourcedatasetsdataset-idreusesreuse-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Reuses
      - Reuse
      - Id
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