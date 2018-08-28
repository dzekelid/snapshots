---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Copy Snapshot
  version: 1.0.0
  description: Makes a copy of an existing snapshot.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CopySnapshot:
    get:
      summary: Copy Snapshot
      description: Makes a copy of an existing snapshot.
      operationId: copySnapshot
      x-api-path-slug: actioncopysnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotName
        description: The name of an existing snapshot from which to make a copy
        type: string
      - in: query
        name: TargetBucket
        description: The Amazon S3 bucket to which the snapshot is exported
        type: string
      - in: query
        name: TargetSnapshotName
        description: A name for the snapshot copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateSnapshot:
    get:
      summary: Create Snapshot
      description: |-
        Creates a copy of an entire cache cluster or replication group at a
                    specific moment in time.
      operationId: createSnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: CacheClusterId
        description: The identifier of an existing cache cluster
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier of an existing replication group
        type: string
      - in: query
        name: SnapshotName
        description: A name for the snapshot being created
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteSnapshot:
    get:
      summary: Delete Snapshot
      description: Deletes an existing snapshot.
      operationId: deleteSnapshot
      x-api-path-slug: actiondeletesnapshot-get
      parameters:
      - in: query
        name: SnapshotName
        description: The name of the snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeSnapshots:
    get:
      summary: Describe Snapshots
      description: Returns information about cache cluster or replication group snapshots.
      operationId: describeSnapshots
      x-api-path-slug: actiondescribesnapshots-get
      parameters:
      - in: query
        name: CacheClusterId
        description: A user-supplied cluster identifier
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ReplicationGroupId
        description: A user-supplied replication group identifier
        type: string
      - in: query
        name: ShowNodeGroupConfig
        description: A Boolean value which if true, the node group (shard) configuration
          is included in the snapshot description
        type: string
      - in: query
        name: SnapshotName
        description: A user-supplied name of the snapshot
        type: string
      - in: query
        name: SnapshotSource
        description: If set to system, the output shows snapshots that were automatically
          created by ElastiCache
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