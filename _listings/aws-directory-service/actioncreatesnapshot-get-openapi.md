---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Create Snapshot
  version: 1.0.0
  description: Creates a snapshot of a Simple AD or Microsoft AD directory in the
    AWS cloud.
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
  /?Action=DescribeSnapshots:
    get:
      summary: Describe Snapshots
      description: Obtains information about the directory snapshots that belong to
        this account.
      operationId: describeSnapshots
      x-api-path-slug: actiondescribesnapshots-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to retrieve snapshot
          information
        type: string
      - in: query
        name: Limit
        description: The maximum number of objects to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeSnapshotsResult
        type: string
      - in: query
        name: SnapshotIds
        description: A list of identifiers of the snapshots to obtain the information
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=GetSnapshotLimits:
    get:
      summary: Get Snapshot Limits
      description: Obtains the manual snapshot limits for a directory.
      operationId: getSnapshotLimits
      x-api-path-slug: actiongetsnapshotlimits-get
      parameters:
      - in: query
        name: DirectoryId
        description: Contains the identifier of the directory to obtain the limits
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RestoreFromSnapshot:
    get:
      summary: Restore From Snapshot
      description: Restores a directory using an existing directory snapshot.
      operationId: restoreFromSnapshot
      x-api-path-slug: actionrestorefromsnapshot-get
      parameters:
      - in: query
        name: SnapshotId
        description: The identifier of the snapshot to restore from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateSnapshot:
    get:
      summary: Create Snapshot
      description: Creates a snapshot of a Simple AD or Microsoft AD directory in
        the AWS cloud.
      operationId: createSnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory of which to take a snapshot
        type: string
      - in: query
        name: Name
        description: The descriptive name to apply to the snapshot
        type: string
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