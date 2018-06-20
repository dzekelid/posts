---
swagger: "2.0"
x-collection-name: Tumblr
x-complete: 0
info:
  title: Tumblr Get Blog Base Hostname Adds Submission
  description: Retrieves submission posts.
  version: 1.0.0
host: api.tumblr.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blog/{base-hostname}/posts/{type}:
    get:
      summary: Get Blog Base Hostname Adds Type
      description: Retrieves published posts.
      operationId: blog.base_hostname.posts.type.get
      x-api-path-slug: blogbasehostnamepoststype-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: format
        description: Specifies the post format to return, other than HTML
      - in: query
        name: id
        description: A specific post ID
      - in: query
        name: limit
        description: 'The number of posts to return: 120, inclusive'
      - in: query
        name: notes_info
        description: Indicates whether to return notes information (specify true or
          false)
      - in: query
        name: offset
        description: Post number to start at
      - in: query
        name: reblog_info
        description: Indicates whether to return reblog information (specify true
          or false)
      - in: query
        name: tag
        description: Limits the response to posts with the specified tag
      - in: path
        name: type
        description: The type of post to return
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Type
  /blog/{base-hostname}/posts/queue:
    get:
      summary: Get Blog Base Hostname Adds Queue
      description: Retrieves queued posts.
      operationId: blog.base_hostname.posts.queue.get
      x-api-path-slug: blogbasehostnamepostsqueue-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Queue
  /blog/{base-hostname}/posts/draft:
    get:
      summary: Get Blog Base Hostname Adds Draft
      description: Retrieves draft posts.
      operationId: blog.base_hostname.posts.draft.get
      x-api-path-slug: blogbasehostnamepostsdraft-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Draft
  /blog/{base-hostname}/posts/submission:
    get:
      summary: Get Blog Base Hostname Adds Submission
      description: Retrieves submission posts.
      operationId: blog.base_hostname.posts.submission.get
      x-api-path-slug: blogbasehostnamepostssubmission-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Submission
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