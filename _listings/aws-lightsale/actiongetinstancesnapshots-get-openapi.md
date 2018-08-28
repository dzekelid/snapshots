---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Instance Snapshots
  version: 1.0.0
  description: Returns all instance snapshots for the user's account.
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
  /?Action=CreateInstanceSnapshot:
    get:
      summary: Create Instance Snapshot
      description: |-
        Creates a snapshot of a specific virtual private server, or
                instance.
      operationId: createInstanceSnapshot
      x-api-path-slug: actioncreateinstancesnapshot-get
      parameters:
      - in: query
        name: instanceName
        description: The Lightsail instance on which to base your snapshot
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name for your new snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteInstanceSnapshot:
    get:
      summary: Delete Instance Snapshot
      description: |-
        Deletes a specific snapshot of a virtual private server (or
                instance).
      operationId: deleteInstanceSnapshot
      x-api-path-slug: actiondeleteinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshot:
    get:
      summary: Get Instance Snapshot
      description: Returns information about a specific instance snapshot.
      operationId: getInstanceSnapshot
      x-api-path-slug: actiongetinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot for which you are requesting information
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