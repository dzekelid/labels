---
name: Ship Station
x-slug: ship-station
description: ShipStation is a web-based shipping solution that streamlines the order
  fulfillment process for your online business. ShipStation consolidates orders from
  over 70 ecommerce channels, creates shipping labels, packing slips, and pick lists
  in batch, communicates tracking information to your customers, provides endless
  automation, filters, and views, wireless printing, a mobile app, and a lot more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Labels
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/ship-station/apis.md
specificationVersion: "0.14"
apis:
- name: Ship Station Developer Portal - Create Shipment Label
  x-api-slug: shipmentscreatelabel-post
  description: "Creates a shipping label.  The ``labelData`` field returned in the
    response is a base64 encoded PDF value. Simply decode and save the output as a
    PDF file to retrieve a printable label.  The body of this request has the following
    attributes:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n
    ``carrierCode`` | string, required | Identifies the carrier to be used for this
    label.\n ``serviceCode`` | string, required | Identifies the shipping service
    to be used for this label.\n ``packageCode`` | string, required | Identifies the
    packing type that should be used for this label.\n ``confirmation`` | string,
    optional | Identifies the delivery confirmation type to be used for this label.\n
    ``shipDate`` | string, required | The date the shipment will be shipped.\n ``weight``
    | Weight, required | Shipment's weight.  Use the [**Weight**](https://www.shipstation.com/developer-api/#/reference/model-weight)
    model.\n ``dimensions`` | Dimensions, optional | Shipment's dimensions.  Use the
    [**Dimensions**](https://www.shipstation.com/developer-api/#/reference/model-dimensions)
    model.\n ``shipFrom`` | Address, required | Address indicating shipment's origin.
    \ Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n ``shipTo`` | Address, required | Address indicating shipment's destination.
    \ Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n ``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
    information associated with this order.  \n ``internationalOptions`` | InternationalOptions,
    optional | Customs information that can be used to generate customs documents
    for international orders.  Use the [**InternationalOptions**](https://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
    model.\n ``advancedOptions`` | AdvancedOptions, optional | Various advanced options
    that may be available depending on the shipping carrier that is used to ship the
    order.  Use the [**AdvancedOptions**](https://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
    model. \n ``testLabel`` | boolean, optional | Specifies whether a test label should
    be created. Default value: false."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/ship-station/shipmentscreatelabel-post-openapi.md
- name: Ship Station Developer Portal - Void Label
  x-api-slug: shipmentsvoidlabel-post
  description: |-
    Voids the specified label by shipmentId.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``shipmentId`` | number, required | ID of the shipment to void.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/ship-station/shipmentsvoidlabel-post-openapi.md
- name: Ship Station Developer Portal - Void Label
  x-api-slug: shipmentsvoidlabel-post
  description: |-
    Voids the specified label by shipmentId.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``shipmentId`` | number, required | ID of the shipment to void.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/ship-station/shipmentsvoidlabel-post-openapi.md
- name: Ship Station Developer Portal - Create Shipment Label
  x-api-slug: shipmentscreatelabel-post
  description: "Creates a shipping label.  The ``labelData`` field returned in the
    response is a base64 encoded PDF value. Simply decode and save the output as a
    PDF file to retrieve a printable label.  The body of this request has the following
    attributes:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n
    ``carrierCode`` | string, required | Identifies the carrier to be used for this
    label.\n ``serviceCode`` | string, required | Identifies the shipping service
    to be used for this label.\n ``packageCode`` | string, required | Identifies the
    packing type that should be used for this label.\n ``confirmation`` | string,
    optional | Identifies the delivery confirmation type to be used for this label.\n
    ``shipDate`` | string, required | The date the shipment will be shipped.\n ``weight``
    | Weight, required | Shipment's weight.  Use the [**Weight**](https://www.shipstation.com/developer-api/#/reference/model-weight)
    model.\n ``dimensions`` | Dimensions, optional | Shipment's dimensions.  Use the
    [**Dimensions**](https://www.shipstation.com/developer-api/#/reference/model-dimensions)
    model.\n ``shipFrom`` | Address, required | Address indicating shipment's origin.
    \ Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n ``shipTo`` | Address, required | Address indicating shipment's destination.
    \ Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n ``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
    information associated with this order.  \n ``internationalOptions`` | InternationalOptions,
    optional | Customs information that can be used to generate customs documents
    for international orders.  Use the [**InternationalOptions**](https://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
    model.\n ``advancedOptions`` | AdvancedOptions, optional | Various advanced options
    that may be available depending on the shipping carrier that is used to ship the
    order.  Use the [**AdvancedOptions**](https://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
    model. \n ``testLabel`` | boolean, optional | Specifies whether a test label should
    be created. Default value: false."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/ship-station/shipmentscreatelabel-post-openapi.md
x-common:
- type: x-website
  url: http://bit.ly/_ShipStation
- type: x-api-gallery
  url: http://server.density.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ship.station.stack.network
- type: x-blog
  url: https://www.shipstation.com/blog/
- type: x-developer
  url: https://shipstation.docs.apiary.io/#
- type: x-github
  url: https://github.com/shipstation
- type: x-partners
  url: https://www.shipstation.com/partners/
- type: x-pricing
  url: https://www.shipstation.com/pricing/
- type: x-twitter
  url: https://twitter.com/ShipStation
- type: x-website
  url: http://shipstation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---