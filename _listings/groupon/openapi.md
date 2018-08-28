swagger: "2.0"
x-collection-name: Groupon
x-complete: 1
info:
  title: Groupon API2
  description: put-all-those-great-ideas-for-groupon-improvements-extensions-and-multipleplatform-interfaces-to-work-
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
    get:
      summary: Get Deals Deal Adds. Format
      description: Returns the lists of all the discussion posts for the specified
        deal.
      operationId: getDealsDealAdds.Format
      x-api-path-slug: dealsdeal-idposts-format-get
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Deal
      - Posts
      - Format