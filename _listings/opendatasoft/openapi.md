---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 1
info:
  title: OpenDataSoft
  description: opendatasoft-is-a-cloudbased-turnkey-platform-for-data-publishing-and-api-management--its-interface-is-intuitively-designed-to-empower-anyone-regardless-of-technical-skills-to-upload-easytounderstand-open-data-or-to-even-share-data-within-an-admi---
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
  /{source}/datasets/{dataset_id}/snapshots:
    get:
      summary: Get Source Datasets Dataset Snapshots
      description: List of all snapshots for this dataset.
      operationId: getDatasetSnapshots
      x-api-path-slug: sourcedatasetsdataset-idsnapshots-get
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
      - Snapshots
  /{source}/datasets/{dataset_id}/snapshots/{snapshot_id}:
    get:
      summary: Get Source Datasets Dataset Snapshots Snapshot
      description: List of all snapshots for this dataset.
      operationId: downloadDatasetSnapshot
      x-api-path-slug: sourcedatasetsdataset-idsnapshotssnapshot-id-get
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
      - Snapshots
      - Snapshot
      - Id
---