swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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