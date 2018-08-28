swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/snapshots:
    get:
      summary: Telemetry Snapshots
      description: Telemetry snapshots.
      operationId: Devices62976d30B6dc40f18422Ccc367572101SnapshotsGet
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101snapshots-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: fields
      responses:
        200:
          description: OK
      tags:
      - Telemetry
      - Snapshots