---
swagger: "2.0"
x-collection-name: Tumblr
x-complete: 1
info:
  title: Tumblr
  description: ntshare-photos-mobile-apps-and-social-network-using-tumblrs-apis-n----
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
---