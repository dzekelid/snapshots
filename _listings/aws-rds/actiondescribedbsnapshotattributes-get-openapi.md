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
  /?Action=DescribeDBSnapshots:
    get:
      summary: Describe D B Snapshots
      description: Returns information about DB snapshots.
      operationId: describedbsnapshots
      x-api-path-slug: actiondescribedbsnapshots-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The ID of the DB instance to retrieve the list of DB snapshots
          for
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: A specific DB snapshot identifier to describe
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: IncludePublic
        description: Set this value to true to include manual DB snapshots that are
          public and can be copied or restored           by any AWS account, otherwise
          set this value to false
        type: string
      - in: query
        name: IncludeShared
        description: Set this value to true to include shared manual DB snapshots
          from other           AWS accounts that this AWS account has been given permission
          to copy or restore, otherwise set this value to false
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBSnapshots
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=ModifyDBSnapshotAttribute:
    get:
      summary: Modify D B Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB snapshot.
      operationId: modifydbsnapshotattribute
      x-api-path-slug: actionmodifydbsnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB snapshot attribute to modify
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to modify the attributes for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB snapshot attributes to add to the attribute specified
          by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RestoreDBClusterFromSnapshot:
    get:
      summary: Restore D B Cluster From Snapshot
      description: Creates a new DB cluster from a DB cluster snapshot.
      operationId: restoredbclusterfromsnapshot
      x-api-path-slug: actionrestoredbclusterfromsnapshot-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: Provides the list of EC2 Availability Zones that instances in
          the restored DB cluster can be created in
        type: string
      - in: query
        name: DatabaseName
        description: The database name for the restored DB cluster
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to create from the DB cluster snapshot
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name of the DB subnet group to use for the new DB cluster
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new DB cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version of the database engine to use for the new DB cluster
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier to use when restoring an encrypted DB
          cluster from a DB cluster snapshot
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to use for the restored DB cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the new DB cluster accepts connections
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier for the DB cluster snapshot to restore from
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the restored DB cluster
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of VPC security groups that the new DB cluster will belong
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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