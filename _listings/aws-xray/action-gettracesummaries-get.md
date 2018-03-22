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
  /?Action=GetTraceSummaries:
    get:
      summary: ' Get Trace Summaries '
      description: |-
        Retrieves IDs and metadata for traces available for a specified time frame using an
              optional filter
      operationId: getTraceSummaries
      parameters:
      - in: query
        name: EndTime
        description: The end of the time frame for which to retrieve traces
        type: string
      - in: query
        name: FilterExpression
        description: Specify a filter expression to retrieve trace summaries for services
          or requests that      meet certain requirements
        type: string
      - in: query
        name: NextToken
        description: Specify the pagination token returned by a previous request to
          retrieve the next page      of results
        type: string
      - in: query
        name: Sampling
        description: Set to true to get summaries for only a subset of available      traces
        type: string
      - in: query
        name: StartTime
        description: The start of the time frame for which to retrieve traces
        type: string
      responses:
        200:
          description: OK
      tags:
      - trace summaries
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