---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Delete Labels Key . Format
  version: 1.0.0
  description: |-
    When applications are provided, this endpoint will remove those applications from the label.

    When no applications are provided, this endpoint will remove the label.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /labels/{key}.{format}:
    delete:
      summary: Delete Labels Key . Format
      description: |-
        When applications are provided, this endpoint will remove those applications from the label.

        When no applications are provided, this endpoint will remove the label.
      operationId: deleteLabelsKey.Format
      x-api-path-slug: labelskey-format-delete
      parameters:
      - in: path
        name: key
        description: Label key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Labels
      - Key
      - .
      - Format
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