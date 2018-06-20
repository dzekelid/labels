---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Labels
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Labels. Format
  x-api-slug: new-relic
  description: This API endpoint returns a paginated list of the labels available
    for the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels.{format}
  tags: Labels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/new-relic/labels-format-get-openapi.md
- name: New Relic Put Labels. Format
  x-api-slug: new-relic
  description: "This API endpoint will create a new label with the provided category
    and name.\n\nInclude the application and server IDs to which the label should
    be applied in the corresponding arrays.\nYou may omit the \u201Clinks\u201D or
    \u201Cservers\u201D arrays, if not needed.\n\nSee our documentation for a discussion
    on obtaining \napplication \nand \nserver IDs."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels.{format}
  tags: Labels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/new-relic/labels-format-put-openapi.md
- name: New Relic Delete Labels Key . Format
  x-api-slug: new-relic
  description: |-
    When applications are provided, this endpoint will remove those applications from the label.

    When no applications are provided, this endpoint will remove the label.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels/{key}.{format}
  tags: Labels, Key, ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/new-relic/labelskey-format-delete-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic???s digital intelligence platform lets developers, ops, and
    tech teams measure and monitor the performance of their applications and infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---