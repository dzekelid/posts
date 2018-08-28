---
swagger: "2.0"
x-collection-name: Vestorly
x-complete: 0
info:
  title: Vestorly Get Posts
  description: Query all posts
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts:
    get:
      summary: Get Posts
      description: Query all posts
      operationId: findPosts
      x-api-path-slug: posts-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: external_url
        description: Filter by External URL
      - in: query
        name: is_published
        description: Filter by is_published boolean
      - in: query
        name: text_query
        description: Filter post by parameters
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Posts
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