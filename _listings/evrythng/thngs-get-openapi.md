---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /thngs (O)
  description: OPERATOR reads the list of all thngs in the account.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /thngs:
    get:
      summary: /thngs (O)
      description: OPERATOR reads the list of all thngs in the account.
      operationId: ThngsGet
      x-api-path-slug: thngs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Thngs
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