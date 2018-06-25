---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
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
---