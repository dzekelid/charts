---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting
    and Reporting Effluent Charts Download Service
  description: Downloads tabular Discharge Monitoring Report (DMR) and compliance
    data for one NPDES permit as a CSV.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 1.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /eff_rest_services.download_effluent_chart:
    get:
      summary: Effluent Charts Download Service
      description: Downloads tabular Discharge Monitoring Report (DMR) and compliance
        data for one NPDES permit as a CSV.
      operationId: downloads-tabular-discharge-monitoring-report-dmr-and-compliance-data-for-one-npdes-permit-as-a-csv-
      x-api-path-slug: eff-rest-services-download-effluent-chart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Effluent
      - Charts
      - Download
      - Service
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