---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Delete Snapshot
  version: 1.0.0
  description: Deletes a directory snapshot.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteSnapshot:
    get:
      summary: Delete Snapshot
      description: Deletes a directory snapshot.
      operationId: deleteSnapshot
      x-api-path-slug: actiondeletesnapshot-get
      parameters:
      - in: query
        name: SnapshotId
        description: The identifier of the directory snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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