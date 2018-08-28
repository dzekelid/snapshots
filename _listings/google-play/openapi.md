swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
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