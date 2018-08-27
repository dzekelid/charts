swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 1
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking
    Water Act
  description: enforcement-and-compliance-history-online-echo-is-a-tool-developed-and-maintained-by-epas-office-of-enforcement-and-compliance-assurance-for-public-use--echo-provides-integrated-compliance-and-enforcement-information-for-about-800000-regulated-facilities-nationwide-brbrsdw-rest-services-provides-multiple-service-endpoints-each-with-specific-capabilities-to-search-and-retrieve-data-on-public-water-systems-regulated-under-the-safe-drinking-water-act-sdwa--the-returned-results-reflect-data-drawn-from-epas-federal-safe-drinking-water-information-system-sdwis-database-brbrthe-get-systems-get-qid-and-get-download-end-points-are-meant-to-be-used-together-brbrthe-recommended-use-scenario-for-get-systems-get-qid-and-get-downoad-isbrbrb1bnbsp-use-get-systems-to-validate-passed-query-parameters-obtain-summary-statistics-and-to-obtain-a-query-id-qid---qids-are-time-sensitive-and-will-be-valid-for-approximately-30-minutes-brb2bnbsp-use-get-qid-with-the-returned-qid-to-paginate-through-arrays-of-water-system-results-brb3bnbsp-use-get-download-with-the-returned-qid-to-generate-a-comma-separated-value-csv-file-of-water-system-information-that-meets-the-qid-query-criteria-brbruse-the-qcolumns-parameter-to-customize-your-search-results---use-the-metdata-service-endpoint-for-a-list-of-available-output-objects-their-column-ids-and-their-definitions-to-help-you-build-your-customized-output--brbradditional-echo-resourcesnbspnbsp-a-hrefhttpsecho-epa-govtoolswebservicesweb-servicesa-a-hrefhttpsecho-epa-govresourcesechodataaboutthedataabout-echos-dataa-a-hrefhttpsecho-epa-govtoolsdatadownloadsdata-downloadsabr
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
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