---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Create Instances From Snapshot
  version: 1.0.0
  description: |-
    Uses a specific snapshot as a blueprint for creating one or more new instances that are
          based on that identical configuration.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetInstanceSnapshots:
    get:
      summary: Get Instance Snapshots
      description: Returns all instance snapshots for the user's account.
      operationId: getInstanceSnapshots
      x-api-path-slug: actiongetinstancesnapshots-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instance snapshots      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstancesFromSnapshot:
    get:
      summary: Create Instances From Snapshot
      description: |-
        Uses a specific snapshot as a blueprint for creating one or more new instances that are
              based on that identical configuration.
      operationId: createInstancesFromSnapshot
      x-api-path-slug: actioncreateinstancesfromsnapshot-get
      parameters:
      - in: query
        name: availabilityZone
        description: The Availability Zone where you want to create your instances
        type: string
      - in: query
        name: bundleId
        description: The bundle of specification information for your virtual private
          server (or        instance), including the pricing plan (e
        type: string
      - in: query
        name: instanceNames
        description: The names for your new instances
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name of the instance snapshot on which you are basing your
          new instances
        type: string
      - in: query
        name: keyPairName
        description: The name for your key pair
        type: string
      - in: query
        name: userData
        description: You can create a launch script that configures a server with
          additional user data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
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