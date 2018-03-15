---
swagger: "2.0"
info:
  title: AWS X-Ray API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutTraceSegments&k=1:
    get:
      summary: ' Put Trace Segments '
      description: Uploads segment documents to AWS X-Ray
      operationId: putTraceSegments
      parameters:
      - in: query
        name: TraceSegmentDocuments
        description: A JSON document defining one or more segments or subsegments
        type: string
      responses:
        200:
          description: OK
      tags:
      - trace segments
definitions: []
x-collection-name: AWS X-Ray
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