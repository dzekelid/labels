---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Put Labels. Format
  version: 1.0.0
  description: "This API endpoint will create a new label with the provided category
    and name.\n\nInclude the application and server IDs to which the label should
    be applied in the corresponding arrays.\nYou may omit the \u201Clinks\u201D or
    \u201Cservers\u201D arrays, if not needed.\n\nSee our documentation for a discussion
    on obtaining \napplication \nand \nserver IDs."
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