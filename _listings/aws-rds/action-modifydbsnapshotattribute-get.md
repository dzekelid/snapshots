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
  /?Action=ModifyDBSnapshotAttribute&k=1:
    get:
      summary: Modify D B Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB snapshot
      operationId: modifydbsnapshotattribute
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