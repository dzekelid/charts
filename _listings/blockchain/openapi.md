---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain Info
  description: use-blockchains-apis-at-no-cost-to-help-you-start-building-bitcoin-apps-
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
---