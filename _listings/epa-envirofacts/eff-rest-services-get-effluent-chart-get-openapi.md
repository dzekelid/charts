---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting
    and Reporting Detailed Effluent Chart Service
  description: Discharge Monitoring Report (DMR) data supporting each effluent chart
    for one NPDES permit. Includes Discharge Monitoring Reports and NPDES Violations.
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
  /eff_rest_services.get_summary_chart:
    get:
      summary: Summary Effluent Chart Service
      description: Summary of compliance status each outfall and parameter for one
        NPDES permit. Provides the current compliance status and overall compliance
        status for the date range of interest. This service supports the Summary Matrix
        on the Effluent Charts.
      operationId: summary-of-compliance-status-each-outfall-and-parameter-for-one-npdes-permit--provides-the-current-c
      x-api-path-slug: eff-rest-services-get-summary-chart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Summary
      - Effluent
      - Chart
      - Service
  /eff_rest_services.get_effluent_chart:
    get:
      summary: Detailed Effluent Chart Service
      description: Discharge Monitoring Report (DMR) data supporting each effluent
        chart for one NPDES permit. Includes Discharge Monitoring Reports and NPDES
        Violations.
      operationId: discharge-monitoring-report-dmr-data-supporting-each-effluent-chart-for-one-npdes-permit--includes-d
      x-api-path-slug: eff-rest-services-get-effluent-chart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Effluent
      - Chart
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