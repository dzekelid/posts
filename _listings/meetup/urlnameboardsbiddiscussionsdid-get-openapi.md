---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Discussion Posts
  description: Listing Group discussion posts
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/boards/:bid/discussions/:did:
    get:
      summary: Discussion Posts
      description: Listing Group discussion posts
      operationId: boards
      x-api-path-slug: urlnameboardsbiddiscussionsdid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discussions
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