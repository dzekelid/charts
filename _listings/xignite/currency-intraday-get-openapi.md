---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Currencies Get Currency Intraday Chart
  description: Draw a intraday currency chart for a time range
  version: 1.0.0
host: www.xignite.com/xCurrencies.json
basePath: /XigniteCurrencies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ', Bars':
    get:
      summary: Get Chart Bars
      description: Returns a set of partial bars for a stock and a time range during
        the trading day.
      operationId: GetChartBars
      x-api-path-slug: bars-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Bars
  Currency, , Custom:
    get:
      summary: Get Currency Chart Custom
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustom
      x-api-path-slug: currency--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Chart
      - Custom
  Currency, , Custom, Binary:
    get:
      summary: Get Currency Chart Custom Binary
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustombinary
      x-api-path-slug: currency--custom-binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Chart
      - Custom
      - Binary
  'Currency, ':
    get:
      summary: Get Currency Chart
      description: Draw a historical currency chart for a date range.
      operationId: postGetcurrencychart
      x-api-path-slug: currency-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Chart
  Currency, , Binary:
    get:
      summary: Get Currency Chart Binary
      description: Draw a historical currency chart for a date range in binary format.
      operationId: postGetcurrencychartbinary
      x-api-path-slug: currency--binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Chart
      - Binary
  'Currency, Intraday, ':
    get:
      summary: Get Currency Intraday Chart
      description: Draw a intraday currency chart for a time range
      operationId: postGetcurrencyintradaychart
      x-api-path-slug: currency-intraday-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Intraday
      - Chart
  Currency, Intraday, , Custom, Binary:
    get:
      summary: Get Currency Intraday Chart Custom Binary
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustombinary
      x-api-path-slug: currency-intraday--custom-binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Intraday
      - Chart
      - Custom
      - Binary
  Currency, Intraday, , Custom:
    get:
      summary: Get Currency Intraday Chart Custom
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustom
      x-api-path-slug: currency-intraday--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Currency
      - Intraday
      - Chart
      - Custom
  ', Design':
    get:
      summary: Get Chart Design
      description: Returns the default design class for the currency Chart.
      operationId: postGetchartdesign
      x-api-path-slug: design-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Design
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