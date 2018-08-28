swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
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