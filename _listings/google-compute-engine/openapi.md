swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 1
info:
  title: Compute Engine
  description: creates-and-runs-virtual-machines-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/snapshots:
    get:
      summary: Get Snapshots
      description: Retrieves the list of Snapshot resources contained within the specified
        project.
      operationId: compute.snapshots.list
      x-api-path-slug: projectglobalsnapshots-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /{project}/global/snapshots/{snapshot}:
    delete:
      summary: Delete Snapshot
      description: |-
        Deletes the specified Snapshot resource. Keep in mind that deleting a single snapshot might not necessarily delete all the data on that snapshot. If any data on the snapshot that is marked for deletion is needed for subsequent snapshots, the data will be moved to the next corresponding snapshot.

        For more information, see Deleting snaphots.
      operationId: compute.snapshots.delete
      x-api-path-slug: projectglobalsnapshotssnapshot-delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: snapshot
        description: Name of the Snapshot resource to delete
      responses:
        200:
          description: OK
      tags:
      - Snapshot
    get:
      summary: Get Snapshot
      description: Returns the specified Snapshot resource. Get a list of available
        snapshots by making a list() request.
      operationId: compute.snapshots.get
      x-api-path-slug: projectglobalsnapshotssnapshot-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: snapshot
        description: Name of the Snapshot resource to return
      responses:
        200:
          description: OK
      tags:
      - Snapshot