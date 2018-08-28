---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List item label templates
  description: Lists the ID and name of all item label templates saved in the system.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
      - Templates
  /rest/items/{id}/variations/{variationId}/labels:
    post:
      summary: Get a variation label
      description: Gets a base64 encoded label for the specified variation ID. The
        labelId of the label template must be specified.
      operationId: postRestItemsVariationsVariationLabels
      x-api-path-slug: restitemsidvariationsvariationidlabels-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Label
  /rest/warehouses/locations/{warehouseId}/label:
    get:
      summary: Generate the warehouse location label
      description: Generates the warehouse location label
      operationId: getRestWarehousesLocationsWarehouseLabel
      x-api-path-slug: restwarehouseslocationswarehouseidlabel-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Warehouse
      - Location
      - Label
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