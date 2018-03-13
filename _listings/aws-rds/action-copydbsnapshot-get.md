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
  /?Action=CopyDBSnapshot&k=1:
    get:
      summary: Copy D B Snapshot
      description: Copies the specified DB snapshot
      operationId: copydbsnapshot
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