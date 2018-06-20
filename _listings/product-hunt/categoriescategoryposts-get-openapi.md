---
swagger: "2.0"
x-collection-name: Product Hunt
x-complete: 0
info:
  title: Product Hunt Posts
  description: Get posts by category.
  version: 1.0.0
host: api.producthunt.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories/{category}/posts:
    get:
      summary: Posts
      description: Get posts by category.
      operationId: categories.category.posts.get
      x-api-path-slug: categoriescategoryposts-get
      parameters:
      - in: path
        name: category
      - in: query
        name: days_ago
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Products
      - Services
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