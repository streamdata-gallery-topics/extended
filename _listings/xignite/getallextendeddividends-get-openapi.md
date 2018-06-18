---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get All Extended Dividends
  description: Get all extended dividend for a date range.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetExtendedDividendHistory:
    get:
      summary: Get Extended Dividend History
      description: Get extended dividend history for a stock.
      operationId: postGetextendeddivendhistory
      x-api-path-slug: getextendeddividendhistory-get
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
      - Extended
      - Dividend
      - History
  /GetExtendedDividendHistoryRange:
    get:
      summary: Get Extended Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetextendeddivendhistoryrange
      x-api-path-slug: getextendeddividendhistoryrange-get
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
      - Extended
      - Dividend
      - History
      - Range
  /GetAllExtendedDividends:
    get:
      summary: Get All Extended Dividends
      description: Get all extended dividend for a date range.
      operationId: postGetallextendeddivends
      x-api-path-slug: getallextendeddividends-get
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
      - Extended
      - Dividends
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