---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Delete Snapshot
  version: 1.0.0
  description: Deletes the specified snapshot.
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
      description: Creates a snapshot of an EBS volume and stores it in Amazon S3.
      operationId: createsnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone in which to create the volume
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the volume should be encrypted
        type: string
      - in: query
        name: Iops
        description: Only valid for Provisioned IOPS SSD volumes
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) customer
          master key (CMK) to use when creating the encrypted      volume
        type: string
      - in: query
        name: Size
        description: The size of the volume, in GiBs
        type: string
      - in: query
        name: SnapshotId
        description: The snapshot from which to create the volume
        type: string
      - in: query
        name: VolumeType
        description: The volume type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=DeleteSnapshot:
    get:
      summary: Delete Snapshot
      description: Deletes the specified snapshot.
      operationId: deletesnapshot
      x-api-path-slug: actiondeletesnapshot-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=ModifySnapshotAttribute:
    get:
      summary: Modify Snapshot Attribute
      description: Adds or removes permission settings for the specified snapshot.
      operationId: modifysnapshotattribute
      x-api-path-slug: actionmodifysnapshotattribute-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=ResetSnapshotAttribute:
    get:
      summary: Reset Snapshot Attribute
      description: Resets permission settings for the specified snapshot.
      operationId: resetsnapshotattribute
      x-api-path-slug: actionresetsnapshotattribute-get
      parameters:
      - in: query
        name: Domain
        description: Set to vpc to allocate the address for use with instances in
          a VPC
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=ImportSnapshot:
    get:
      summary: Import Snapshot
      description: Describes your import snapshot tasks.
      operationId: importsnapshot
      x-api-path-slug: actionimportsnapshot-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the resulting EBS volume
        type: string
      - in: query
        name: Description
        description: A description of the volume
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      - in: query
        name: Image
        description: The disk image
        type: string
      - in: query
        name: Volume
        description: The volume size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=DescribeSnapshots:
    get:
      summary: Describe Snapshots
      description: Describes one or more of the EBS snapshots available to you.
      operationId: describesnapshots
      x-api-path-slug: actiondescribesnapshots-get
      parameters:
      - in: query
        name: Attribute
        description: The instance attribute
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive Snapshot
  /?Action=CopySnapshot:
    get:
      summary: Copy Snapshot
      description: Copies a point-in-time snapshot of an EBS volume and stores it
        in Amazon S3.
      operationId: copysnapshot
      x-api-path-slug: actioncopysnapshot-get
      parameters:
      - in: query
        name: Description
        description: A description for the snapshot
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive Snapshot
  /?Action=DescribeImportSnapshotTasks:
    get:
      summary: Describe Import Snapshot Tasks
      description: Describes your import snapshot tasks.
      operationId: describeimportsnapshottasks
      x-api-path-slug: actiondescribeimportsnapshottasks-get
      parameters:
      - in: query
        name: Description
        description: A description for the instance being imported
        type: string
      - in: query
        name: DiskImage.N
        description: The disk image
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      - in: query
        name: LaunchSpecification
        description: The launch specification
        type: string
      - in: query
        name: Platform
        description: The instance operating system
        type: string
      responses:
        200:
          description: OK
      tags:
      - Import Snapshot Takss
  /?Action=DescribeSnapshotAttribute:
    get:
      summary: Describe Snapshot Attribute
      description: Describes the specified attribute of the specified snapshot.
      operationId: describesnapshotattribute
      x-api-path-slug: actiondescribesnapshotattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of snapshot results returned by DescribeSnapshots
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeSnapshots
          request where MaxResults was used and the      results exceeded the value
          of that parameter
        type: string
      - in: query
        name: Owner.N
        description: Returns the snapshots owned by the specified owner
        type: string
      - in: query
        name: RestorableBy.N
        description: One or more AWS accounts IDs that can create volumes from the
          snapshot
        type: string
      - in: query
        name: SnapshotId.N
        description: One or more snapshot IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive Snapshot
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