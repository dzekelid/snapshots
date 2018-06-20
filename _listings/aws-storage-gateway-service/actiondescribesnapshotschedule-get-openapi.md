---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe Snapshot Schedule
  version: 1.0.0
  description: Describes the snapshot schedule for the specified gateway volume.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateSnapshot:
    get:
      summary: Create Snapshot
      description: Initiates a snapshot of a volume.
      operationId: createSnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: Textual description of the snapshot that appears in the Amazon
          EC2 console, Elastic         Block Store snapshots panel in the Description
          field, and         in the AWS Storage Gateway snapshot Details pane,            Description
          field
        type: string
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateSnapshotFromVolumeRecoveryPoint:
    get:
      summary: Create Snapshot From Volume Recovery Point
      description: Initiates a snapshot of a gateway from a volume recovery point.
      operationId: createSnapshotFromVolumeRecoveryPoint
      x-api-path-slug: actioncreatesnapshotfromvolumerecoverypoint-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteSnapshotSchedule:
    get:
      summary: Delete Snapshot Schedule
      description: Deletes a snapshot of a volume.
      operationId: deleteSnapshotSchedule
      x-api-path-slug: actiondeletesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeSnapshotSchedule:
    get:
      summary: Describe Snapshot Schedule
      description: Describes the snapshot schedule for the specified gateway volume.
      operationId: describeSnapshotSchedule
      x-api-path-slug: actiondescribesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
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