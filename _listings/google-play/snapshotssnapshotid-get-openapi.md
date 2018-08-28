---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Get Snapshot
  version: 1.0.0
  description: Retrieves the metadata for a given snapshot ID.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /snapshots/{snapshotId}:
    get:
      summary: Get Snapshot
      description: Retrieves the metadata for a given snapshot ID.
      operationId: games.snapshots.get
      x-api-path-slug: snapshotssnapshotid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: snapshotId
        description: The ID of the snapshot
      responses:
        200:
          description: OK
      tags:
      - Snapshot
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