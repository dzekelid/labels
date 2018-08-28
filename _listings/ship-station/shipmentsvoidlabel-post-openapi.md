---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Void Label
  description: |-
    Voids the specified label by shipmentId.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``shipmentId`` | number, required | ID of the shipment to void.
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipments/createlabel:
    post:
      summary: Create Shipment Label
      description: "Creates a shipping label.  The ``labelData`` field returned in
        the response is a base64 encoded PDF value. Simply decode and save the output
        as a PDF file to retrieve a printable label.  The body of this request has
        the following attributes:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n
        ``carrierCode`` | string, required | Identifies the carrier to be used for
        this label.\n ``serviceCode`` | string, required | Identifies the shipping
        service to be used for this label.\n ``packageCode`` | string, required |
        Identifies the packing type that should be used for this label.\n ``confirmation``
        | string, optional | Identifies the delivery confirmation type to be used
        for this label.\n ``shipDate`` | string, required | The date the shipment
        will be shipped.\n ``weight`` | Weight, required | Shipment's weight.  Use
        the [**Weight**](https://www.shipstation.com/developer-api/#/reference/model-weight)
        model.\n ``dimensions`` | Dimensions, optional | Shipment's dimensions.  Use
        the [**Dimensions**](https://www.shipstation.com/developer-api/#/reference/model-dimensions)
        model.\n ``shipFrom`` | Address, required | Address indicating shipment's
        origin.  Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
        model.\n ``shipTo`` | Address, required | Address indicating shipment's destination.
        \ Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
        model.\n ``insuranceOptions`` | InsuranceOptions, optional | The shipping
        insurance information associated with this order.  \n ``internationalOptions``
        | InternationalOptions, optional | Customs information that can be used to
        generate customs documents for international orders.  Use the [**InternationalOptions**](https://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
        model.\n ``advancedOptions`` | AdvancedOptions, optional | Various advanced
        options that may be available depending on the shipping carrier that is used
        to ship the order.  Use the [**AdvancedOptions**](https://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
        model. \n ``testLabel`` | boolean, optional | Specifies whether a test label
        should be created. Default value: false."
      operationId: shipments.createlabel.post
      x-api-path-slug: shipmentscreatelabel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipment
      - Label
  /shipments/voidlabel:
    post:
      summary: Void Label
      description: |-
        Voids the specified label by shipmentId.  The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
         ``shipmentId`` | number, required | ID of the shipment to void.
      operationId: shipments.voidlabel.post
      x-api-path-slug: shipmentsvoidlabel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Void
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