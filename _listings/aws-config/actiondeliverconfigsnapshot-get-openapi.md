---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Deliver Config Snapshot
  version: 1.0.0
  description: Schedules delivery of a configuration snapshot to the Amazon S3 bucket
    in the specified delivery channel.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeliverConfigSnapshot:
    get:
      summary: Deliver Config Snapshot
      description: Schedules delivery of a configuration snapshot to the Amazon S3
        bucket in the specified delivery channel.
      operationId: deliverConfigSnapshot
      x-api-path-slug: actiondeliverconfigsnapshot-get
      parameters:
      - in: query
        name: deliveryChannelName
        description: The name of the delivery channel through which the snapshot is
          delivered
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Snapshot
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