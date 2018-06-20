---
swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetectLabels:
    get:
      summary: Detect Labels
      description: |-
        Detects instances of real-world labels within an image (JPEG or PNG)
               provided as input.
      operationId: detectLabels
      x-api-path-slug: actiondetectlabels-get
      parameters:
      - in: query
        name: Image
        description: The input image
        type: string
      - in: query
        name: MaxLabels
        description: Maximum number of labels you want the service to return in the
          response
        type: string
      - in: query
        name: MinConfidence
        description: Specifies the minimum confidence level for the labels to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Labels
---