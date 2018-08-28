swagger: "2.0"
x-collection-name: AWS Simple Queue Service
x-complete: 1
info:
  title: AWS Simple Queue Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemovePermission:
    get:
      summary: Remove Permission
      description: Revokes any permissions in the queue policy that matches the specified
        Label parameter.
      operationId: removePermission
      x-api-path-slug: actionremovepermission-get
      parameters:
      - in: query
        name: Label
        description: The identification of the permission to remove
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which permissions are removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions