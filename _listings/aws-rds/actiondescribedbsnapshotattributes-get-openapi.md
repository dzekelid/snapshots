---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe D B Snapshot Attributes
  version: 1.0.0
  description: Returns a list of DB snapshot attribute names and values for a manual
    DB snapshot.
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
  /?Action=DeleteDBClusterSnapshot:
    get:
      summary: Delete D B Cluster Snapshot
      description: Deletes a DB cluster snapshot.
      operationId: deletedbclustersnapshot
      x-api-path-slug: actiondeletedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DeleteDBSnapshot:
    get:
      summary: Delete D B Snapshot
      description: Deletes a DBSnapshot.
      operationId: deletedbsnapshot
      x-api-path-slug: actiondeletedbsnapshot-get
      parameters:
      - in: query
        name: DBSnapshotIdentifier
        description: The DBSnapshot identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeDBClusterSnapshotAttributes:
    get:
      summary: Describe D B Cluster Snapshot Attributes
      description: Returns a list of DB cluster snapshot attribute names and values
        for a manual DB cluster snapshot.
      operationId: describedbclustersnapshotattributes
      x-api-path-slug: actiondescribedbclustersnapshotattributes-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBClusterSnapshots:
    get:
      summary: Describe D B Cluster Snapshots
      description: Returns information about DB cluster snapshots.
      operationId: describedbclustersnapshots
      x-api-path-slug: actiondescribedbclustersnapshots-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The ID of the DB cluster to retrieve the list of DB cluster snapshots
          for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: A specific DB cluster snapshot identifier to describe
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: IncludePublic
        description: Set this value to true to include manual DB cluster snapshots
          that are public and can be copied             or restored by any AWS account,
          otherwise set this value to false
        type: string
      - in: query
        name: IncludeShared
        description: Set this value to true to include shared manual DB cluster snapshots             from
          other AWS accounts that this AWS account has been given             permission
          to copy or restore, otherwise set this value to false
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusterSnapshots
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SnapshotType
        description: The type of DB cluster snapshots to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBSnapshotAttributes:
    get:
      summary: Describe D B Snapshot Attributes
      description: Returns a list of DB snapshot attribute names and values for a
        manual DB snapshot.
      operationId: describedbsnapshotattributes
      x-api-path-slug: actiondescribedbsnapshotattributes-get
      parameters:
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to describe the attributes
          for
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