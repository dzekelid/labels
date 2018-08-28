swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Orders/{LogicbrokerKey}/ShippingOptions:
    get:
      summary: Get shipping/tracking label options.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Order_GetShippingOptions
      x-api-path-slug: apiv1orderslogicbrokerkeyshippingoptions-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Tracking
      - Label
      - Options