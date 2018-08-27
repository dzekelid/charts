---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 0
info:
  title: Blockchain Info Chart Type
  description: Returns chart types.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  Blockchain,s:
    get:
      summary: Chart Type
      description: Returns chart types.
      operationId: getChartType
      x-api-path-slug: blockchains-get
      parameters:
      - in: path
        name: chart-type
        description: The chart type
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Charts
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