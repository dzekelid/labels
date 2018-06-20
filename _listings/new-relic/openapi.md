---
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
  /labels.{format}:
    get:
      summary: Get Labels. Format
      description: This API endpoint returns a paginated list of the labels available
        for the account.
      operationId: getLabels.Format
      x-api-path-slug: labels-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Labels.
      - Format
    put:
      summary: Put Labels. Format
      description: "This API endpoint will create a new label with the provided category
        and name.\n\nInclude the application and server IDs to which the label should
        be applied in the corresponding arrays.\nYou may omit the \u201Clinks\u201D
        or \u201Cservers\u201D arrays, if not needed.\n\nSee our documentation for
        a discussion on obtaining \napplication \nand \nserver IDs."
      operationId: putLabels.Format
      x-api-path-slug: labels-format-put
      parameters:
      - in: body
        name: label
        description: Label schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Labels.
      - Format
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
---