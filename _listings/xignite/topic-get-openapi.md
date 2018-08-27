---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Statistics Get Topic Chart
  description: Get time-series data and a URL to a chart for a topic.
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
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
      description: Returns the default design class for the statistics Chart.
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
  'Intraday, Future, ':
    get:
      summary: Get Intraday Future Chart
      description: Get a standard intraday price chart for a future contract.
      operationId: postGetintradayfuturechart
      x-api-path-slug: intraday-future-get
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
      - Intraday
      - Future
      - Chart
  Intraday, Future, , Binary:
    get:
      summary: Get Intraday Future Chart Binary
      description: Get a standard intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartbinary
      x-api-path-slug: intraday-future--binary-get
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
      - Intraday
      - Future
      - Chart
      - Binary
  Intraday, Future, , Custom:
    get:
      summary: Get Intraday Future Chart Custom
      description: Get a custom intraday price chart for a future contract.
      operationId: postGetintradayfuturechartcustom
      x-api-path-slug: intraday-future--custom-get
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
      - Intraday
      - Future
      - Chart
      - Custom
  Intraday, Future, , Custom, Binary:
    get:
      summary: Get Intraday Future Chart Custom Binary
      description: Get a custom intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartcustombinary
      x-api-path-slug: intraday-future--custom-binary-get
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
      - Intraday
      - Future
      - Chart
      - Custom
      - Binary
  'Historical, Future, ':
    get:
      summary: Get Historical Future Chart
      description: Get a standard historical price chart for a future contract.
      operationId: postGethistoricalfuturechart
      x-api-path-slug: historical-future-get
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
      - Historical
      - Future
      - Chart
  Historical, Future, , Binary:
    get:
      summary: Get Historical Future Chart Binary
      description: Get a standard historical price chart for a future contract in
        binary format.
      operationId: postGethistoricalfuturechartbinary
      x-api-path-slug: historical-future--binary-get
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
      - Historical
      - Future
      - Chart
      - Binary
  Historical, Future, , Custom:
    get:
      summary: Get Historical Future Chart Custom
      description: Get a custom historical chart for a future contract in binary format.
      operationId: postGethistoricalfuturechartcustom
      x-api-path-slug: historical-future--custom-get
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
      - Historical
      - Future
      - Chart
      - Custom
  Historical, Future, , Custom, Binary:
    get:
      summary: Get Historical Future Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalfuturechartcustombinary
      x-api-path-slug: historical-future--custom-binary-get
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
      - Historical
      - Future
      - Chart
      - Custom
      - Binary
  'Historical, Commodity, ':
    get:
      summary: Get Historical Commodity Chart
      description: Get a historical chart for a commodity.
      operationId: postGethistoricalcommoditychart
      x-api-path-slug: historical-commodity-get
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
      - Historical
      - Commodity
      - Chart
  Historical, Commodity, , Binary:
    get:
      summary: Get Historical Commodity Chart Binary
      description: Get a historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartbinary
      x-api-path-slug: historical-commodity--binary-get
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
      - Historical
      - Commodity
      - Chart
      - Binary
  Historical, Commodity, , Custom:
    get:
      summary: Get Historical Commodity Chart Custom
      description: Get a custom historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartcustom
      x-api-path-slug: historical-commodity--custom-get
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
      - Historical
      - Commodity
      - Chart
      - Custom
  Historical, Commodity, , Custom, Binary:
    get:
      summary: Get Historical Commodity Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalcommoditychartcustombinary
      x-api-path-slug: historical-commodity--custom-binary-get
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
      - Historical
      - Commodity
      - Chart
      - Custom
      - Binary
  Intraday, , Design:
    get:
      summary: Get Intraday Chart Design
      description: Returns the default settings for the intraday future chart.
      operationId: postGetintradaychartdesign
      x-api-path-slug: intraday--design-get
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
      - Intraday
      - Chart
      - Design
  Historical, , Design:
    get:
      summary: Get Historical Chart Design
      description: Returns the default settings for the historical future chart.
      operationId: postGethistoricalchartdesign
      x-api-path-slug: historical--design-get
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
      - Historical
      - Chart
      - Design
  Draw, Rate, , Custom:
    get:
      summary: Draw Rate Chart Custom
      description: Draw a custom rate chart for a date range.
      operationId: postDrawratechartcustom
      x-api-path-slug: draw-rate--custom-get
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
      - Draw
      - Rate
      - Chart
      - Custom
  'Draw, Rate, ':
    get:
      summary: Draw Rate Chart
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechart
      x-api-path-slug: draw-rate-get
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
      - Draw
      - Rate
      - Chart
  Draw, Rate, , Preset:
    get:
      summary: Draw Rate Chart Preset
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechartpreset
      x-api-path-slug: draw-rate--preset-get
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
      - Draw
      - Rate
      - Chart
      - Preset
  'Topic, ':
    get:
      summary: Get Topic Chart
      description: Get time-series data and a URL to a chart for a topic.
      operationId: postGettopicchart
      x-api-path-slug: topic-get
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
      - Topic
      - Chart
  Topic, , Preset:
    get:
      summary: Get Topic Chart Preset
      description: Get a preset chart for a topic.
      operationId: postGettopicchartpreset
      x-api-path-slug: topic--preset-get
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
      - Topic
      - Chart
      - Preset
  Topic, , Custom:
    get:
      summary: Get Topic Chart Custom
      description: Get time-series data and a URL to a custom chart for a topic.
      operationId: postGettopicchartcustom
      x-api-path-slug: topic--custom-get
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
      - Topic
      - Chart
      - Custom
  'Topic, Binary, ':
    get:
      summary: Get Topic Binary Chart
      description: Get time-series and a chart in binary format for a topic.
      operationId: postGettopicbinarychart
      x-api-path-slug: topic-binary-get
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
      - Topic
      - Binary
      - Chart
  Topic, Binary, , Preset:
    get:
      summary: Get Topic Binary Chart Preset
      description: Get time-series and a chart in binary format for a topic.
      operationId: postGettopicbinarychartpreset
      x-api-path-slug: topic-binary--preset-get
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
      - Topic
      - Binary
      - Chart
      - Preset
  Topic, Binary, , Custom:
    get:
      summary: Get Topic Binary Chart Custom
      description: Get time-series and a custom chart in binary format for a topic.
      operationId: postGettopicbinarychartcustom
      x-api-path-slug: topic-binary--custom-get
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
      - Topic
      - Binary
      - Chart
      - Custom
  ', Url':
    get:
      summary: Get Chart Url
      description: Get chart url for a topic.
      operationId: postGetcharturl
      x-api-path-slug: url-get
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
      - Url
  ', Url, Preset':
    get:
      summary: Get Chart Url Preset
      description: Get chart url for a topic.
      operationId: postGetcharturlpreset
      x-api-path-slug: url-preset-get
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
      - Url
      - Preset
  ', Url, Custom':
    get:
      summary: Get Chart Url Custom
      description: Get chart url for a topic.
      operationId: postGetcharturlcustom
      x-api-path-slug: url-custom-get
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
      - Url
      - Custom
  ', Binary':
    get:
      summary: Get Chart Binary
      description: Get chart in binary format for a topic.
      operationId: postGetchartbinary
      x-api-path-slug: binary-get
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
      - Binary
  ', Binary, Preset':
    get:
      summary: Get Chart Binary Preset
      description: Get chart in binary format for a topic.
      operationId: postGetchartbinarypreset
      x-api-path-slug: binary-preset-get
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
      - Binary
      - Preset
  ', Binary, Custom':
    get:
      summary: Get Chart Binary Custom
      description: Get chart in binary format for a topic.
      operationId: postGetchartbinarycustom
      x-api-path-slug: binary-custom-get
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
      - Binary
      - Custom
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