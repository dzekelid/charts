---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns list of movies based on the weekend box office
    revenue.
  description: Returns top 10 box office movies.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Charts/Movies/Boxoffice:
    get:
      summary: Returns list of movies based on the weekend box office revenue.
      description: Returns top 10 box office movies.
      operationId: GetChartMoviesBoxoffice
      x-api-path-slug: chartsmoviesboxoffice-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - Boxoffice
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