---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Create D B Snapshot
  version: 1.0.0
  description: Creates a DBSnapshot.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CopyDBClusterSnapshot:
    get:
      summary: Copy D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: copydbclustersnapshot
      x-api-path-slug: actioncopydbclustersnapshot-get
      parameters:
      - in: query
        name: SourceDBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to copy
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterSnapshotIdentifier
        description: The identifier of the new DB cluster snapshot to create from
          the source DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=CopyDBSnapshot:
    get:
      summary: Copy D B Snapshot
      description: Copies the specified DB snapshot.
      operationId: copydbsnapshot
      x-api-path-slug: actioncopydbsnapshot-get
      parameters:
      - in: query
        name: CopyTags
        description: True to copy all tags from the source DB snapshot to the target
          DB snapshot; otherwise false
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS KMS key ID for an encrypted DB snapshot
        type: string
      - in: query
        name: PreSignedUrl
        description: The URL that contains a Signature Version 4 signed request for
          the CopyDBSnapshot API action in the AWS region that contains the             source
          DB snapshot to copy
        type: string
      - in: query
        name: SourceDBSnapshotIdentifier
        description: The identifier for the source DB snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBSnapshotIdentifier
        description: The identifier for the copied snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateDBClusterSnapshot:
    get:
      summary: Create D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: createdbclustersnapshot
      x-api-path-slug: actioncreatedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster to create a snapshot for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=CreateDBSnapshot:
    get:
      summary: Create D B Snapshot
      description: Creates a DBSnapshot.
      operationId: createdbsnapshot
      x-api-path-slug: actioncreatedbsnapshot-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
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