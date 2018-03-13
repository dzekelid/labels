---
swagger: "2.0"
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
  /?Action=DetectLabels&k=1:
    get:
      summary: ' Detect Labels '
      description: |-
        Detects instances of real-world labels within an image (JPEG or PNG)
               provided as input
      operationId: detectLabels
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
      - labels
definitions: []
x-collection-name: AWS Rekognition
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