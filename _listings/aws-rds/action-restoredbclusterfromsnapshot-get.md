---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RestoreDBClusterFromSnapshot&k=1:
    get:
      summary: Restore D B Cluster From Snapshot
      description: Creates a new DB cluster from a DB cluster snapshot
      operationId: restoredbclusterfromsnapshot
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
      - snapshots
definitions: []
x-collection-name: AWS RDS
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