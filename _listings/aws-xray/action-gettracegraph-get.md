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
  /?Action=GetTraceGraph:
    get:
      summary: ' Get Trace Graph '
      description: Retrieves a service graph for one or more specific trace IDs
      operationId: getTraceGraph
      parameters:
      - in: query
        name: NextToken
        description: Pagination token
        type: string
      - in: query
        name: TraceIds
        description: Trace IDs of requests for which to generate a service graph
        type: string
      responses:
        200:
          description: OK
      tags:
      - trace graph
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