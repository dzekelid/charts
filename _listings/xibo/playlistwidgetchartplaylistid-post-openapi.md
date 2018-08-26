---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Add a Chart Widget
  description: Add a new Chart Widget to the specified playlist
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/chart/{playlistId}:
    post:
      summary: Add a Chart Widget
      description: Add a new Chart Widget to the specified playlist
      operationId: WidgetChartAdd
      x-api-path-slug: playlistwidgetchartplaylistid-post
      parameters:
      - in: formData
        name: backgroundColor
        description: EDIT Only - Background Color
      - in: formData
        name: columnType
        description: EDIT only - Array of Column Types (x-axis, y-axis, series-identifier)
          to assign
      - in: formData
        name: dataSetColumnId
        description: EDIT only - Array of dataSetColumn IDs to assign
      - in: formData
        name: dataSetId
        description: Create Chart Widget using provided dataSetId of an existing dataSet
      - in: formData
        name: duration
        description: EDIT Only - The Chart Duration
      - in: formData
        name: filter
        description: EDIT Only - SQL clause for filter this dataSet
      - in: formData
        name: fontColor
        description: EDIT Only - Font Color
      - in: formData
        name: fontSize
        description: EDIT Only - Font Size
      - in: formData
        name: graphType
        description: EDIT only - Chart Type
      - in: formData
        name: legendPosition
        description: EDIT Only - Where should the Legend be Shown (top, left, right,
          bottom)
      - in: formData
        name: name
        description: Optional Widget Name
      - in: formData
        name: ordering
        description: EDIT Only - SQL clause for how this dataSet should be ordered
      - in: path
        name: playlistId
        description: The playlist ID to add a Widget to
      - in: formData
        name: showLegend
        description: EDIT Only - Should the Legend be Shown
      - in: formData
        name: startYAtZero
        description: EDIT Only - Start the Y-Axis at 0
      - in: formData
        name: title
        description: EDIT Only - Chart title
      - in: formData
        name: updateInterval
        description: EDIT Only - Update interval in minutes
      - in: formData
        name: useDuration
        description: Edit Only - (0, 1) Select 1 only if you will provide duration
          parameter as well
      - in: formData
        name: useFilteringClause
        description: EDIT Only - flag (0,1) Use advanced filter clause - set to 1
          if filter is provided
      - in: formData
        name: useOrderingClause
        description: EDIT Only - flag (0,1) Use advanced order clause - set to 1 if
          ordering is provided
      - in: formData
        name: x-axis-label
        description: EDIT Only - Chart x-axis label
      - in: formData
        name: y-axis-label
        description: EDIT Only - Chart y-axis label
      responses:
        200:
          description: OK
      tags:
      - Chart
      - Widget
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