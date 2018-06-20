---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Enable Snapshot Copy
  version: 1.0.0
  description: |-
    Enables the automatic copy of snapshots from one region to another region for a
                specified cluster.
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
  /?Action=CreateSnapshotCopyGrant:
    get:
      summary: Create Snapshot Copy Grant
      description: |-
        Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                    (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                    destination region.
      operationId: createSnapshotCopyGrant
      x-api-path-slug: actioncreatesnapshotcopygrant-get
      parameters:
      - in: query
        name: KmsKeyId
        description: The unique identifier of the customer master key (CMK) to which
          to grant Amazon Redshift            permission
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
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
  /?Action=DeleteClusterSnapshot:
    get:
      summary: Delete Cluster Snapshot
      description: Deletes the specified manual snapshot.
      operationId: deleteClusterSnapshot
      x-api-path-slug: actiondeleteclustersnapshot-get
      parameters:
      - in: query
        name: SnapshotClusterIdentifier
        description: The unique identifier of the cluster the snapshot was created
          from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The unique identifier of the manual snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteSnapshotCopyGrant:
    get:
      summary: Delete Snapshot Copy Grant
      description: Deletes the specified snapshot copy grant.
      operationId: deleteSnapshotCopyGrant
      x-api-path-slug: actiondeletesnapshotcopygrant-get
      parameters:
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeClusterSnapshots:
    get:
      summary: Describe Cluster Snapshots
      description: |-
        Returns one or more snapshot objects, which contain metadata about your cluster
                    snapshots.
      operationId: describeClusterSnapshots
      x-api-path-slug: actiondescribeclustersnapshots-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster for which information about snapshots
          is            requested
        type: string
      - in: query
        name: EndTime
        description: A time value that requests only snapshots created at or before
          the specified time
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The snapshot identifier of the snapshot about which to return            information
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots for which you are requesting information
        type: string
      - in: query
        name: StartTime
        description: A value that requests only snapshots created at or after the
          specified time
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          snapshots that            are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster snapshots            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeSnapshotCopyGrants:
    get:
      summary: Describe Snapshot Copy Grants
      description: |-
        Returns a list of snapshot copy grants owned by the AWS account in the destination
                    region.
      operationId: describeSnapshotCopyGrants
      x-api-path-slug: actiondescribesnapshotcopygrants-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DisableSnapshotCopy:
    get:
      summary: Disable Snapshot Copy
      description: |-
        Disables the automatic copying of snapshots from one region to another region for a
                    specified cluster.
      operationId: disableSnapshotCopy
      x-api-path-slug: actiondisablesnapshotcopy-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster that you want to
          disable copying of            snapshots to a destination region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=EnableSnapshotCopy:
    get:
      summary: Enable Snapshot Copy
      description: |-
        Enables the automatic copy of snapshots from one region to another region for a
                    specified cluster.
      operationId: enableSnapshotCopy
      x-api-path-slug: actionenablesnapshotcopy-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster to copy snapshots
          from
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region that you want to copy snapshots to
        type: string
      - in: query
        name: RetentionPeriod
        description: The number of days to retain automated snapshots in the destination
          region after            they are copied from the source region
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to use when snapshots of
          an AWS KMS-encrypted            cluster are copied to the destination region
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