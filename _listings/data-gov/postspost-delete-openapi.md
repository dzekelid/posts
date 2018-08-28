---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Delete Post
  description: Delete a given post
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/:
    get:
      summary: Posts
      description: List all posts
      operationId: getPosts
      x-api-path-slug: posts-get
      parameters:
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Posts
    post:
      summary: Add Post
      description: Create a post
      operationId: postPosts
      x-api-path-slug: posts-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{post}/:
    delete:
      summary: Delete Post
      description: Delete a given post
      operationId: deletePostsPost
      x-api-path-slug: postspost-delete
      parameters:
      - in: path
        name: post
        description: The post ID or slug
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