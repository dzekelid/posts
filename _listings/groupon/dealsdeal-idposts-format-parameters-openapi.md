---
swagger: "2.0"
x-collection-name: Groupon
x-complete: 0
info:
  title: Groupon Parameters Deals Deal Adds. Format
  description: Parameters deals deal adds. format.
  version: v2
host: api.groupon.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deals/{deal_id}/posts.{format}:
    parameters:
      summary: Parameters Deals Deal Adds. Format
      description: Parameters deals deal adds. format.
      operationId: parametersDealsDealAdds.Format
      x-api-path-slug: dealsdeal-idposts-format-parameters
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Deal
      - Posts
      - Format
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