---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Posts GetContext
  description: Posts GetContext
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/create.json:
    post:
      summary: Posts Create
      description: Posts Create
      operationId: posts-create
      x-api-path-slug: postscreate-json-post
      parameters:
      - in: query
        name: author_email
        description: Defaults to null                         Email address (defined
          by RFC 5322)
        type: string
      - in: query
        name: author_name
        description: Defaults to null
        type: string
      - in: query
        name: author_url
        description: Defaults to null                         URL (defined by RFC
          3986)
        type: string
      - in: query
        name: date
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: ip_address
        description: Defaults to null                         IP address (defined
          by RFC 5322)
        type: string
      - in: query
        name: message
        type: string
      - in: query
        name: parent
        description: Defaults to null                         Looks up a post by ID
        type: string
      - in: query
        name: state
        description: 'Defaults to null                         Choices: unapproved,
          approved, spam, killed'
        type: string
      - in: query
        name: thread
        description: Defaults to null                         Looks up a thread by
          ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/details.json:
    get:
      summary: Posts Details
      description: Posts Details
      operationId: posts-details
      x-api-path-slug: postsdetails-json-get
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/getContext.json:
    get:
      summary: Posts GetContext
      description: Posts GetContext
      operationId: posts-getcontext
      x-api-path-slug: postsgetcontext-json-get
      parameters:
      - in: query
        name: depth
        description: Defaults to 10                         Minimum value of 1 Maximum
          value of 10
        type: string
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
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