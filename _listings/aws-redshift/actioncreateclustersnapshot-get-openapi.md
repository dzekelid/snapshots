---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Create Cluster Snapshot
  version: 1.0.0
  description: Creates a manual snapshot of the specified cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeSnapshotAccess:
    get:
      summary: Authorize Snapshot Access
      description: |-
        Authorizes the specified AWS customer account to restore the specified
                    snapshot.
      operationId: authorizeSnapshotAccess
      x-api-path-slug: actionauthorizesnapshotaccess-get
      parameters:
      - in: query
        name: AccountWithRestoreAccess
        description: The identifier of the AWS customer account authorized to restore
          the specified            snapshot
        type: string
      - in: query
        name: SnapshotClusterIdentifier
        description: The identifier of the cluster the snapshot was created from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier of the snapshot the account is authorized to restore
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CopyClusterSnapshot:
    get:
      summary: Copy Cluster Snapshot
      description: Copies the specified automated cluster snapshot to a new manual
        cluster snapshot.
      operationId: copyClusterSnapshot
      x-api-path-slug: actioncopyclustersnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotClusterIdentifier
        description: The identifier of the cluster the source snapshot was created
          from
        type: string
      - in: query
        name: SourceSnapshotIdentifier
        description: The identifier for the source snapshot
        type: string
      - in: query
        name: TargetSnapshotIdentifier
        description: The identifier given to the new manual snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateClusterSnapshot:
    get:
      summary: Create Cluster Snapshot
      description: Creates a manual snapshot of the specified cluster.
      operationId: createClusterSnapshot
      x-api-path-slug: actioncreateclustersnapshot-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The cluster identifier for which you want a snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: A unique identifier for the snapshot that you are requesting
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
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