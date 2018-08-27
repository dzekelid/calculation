---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Bonds Get Bond Calculation
  description: Returns Price, Yield, Accrued Interest and other bond analytics data
    for a specific bond reported by the price source selected in the input. Request
    against this operation counts as four hits.
  version: 1.0.0
host: bonds.xignite.com
basePath: xBonds.json/XigniteBonds
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetBondCalculation:
    get:
      summary: Get Bond Calculation
      description: Returns Price, Yield, Accrued Interest and other bond analytics
        data for a specific bond reported by the price source selected in the input.
        Request against this operation counts as four hits.
      operationId: GetBondCalculation
      x-api-path-slug: getbondcalculation-get
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
      - Bond
      - Calculation
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