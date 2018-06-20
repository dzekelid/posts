---
swagger: "2.0"
x-collection-name: Pinboard
x-complete: 0
info:
  title: Pinboard Get Recent Posts
  description: Returns a list of the user's most recent posts, filtered by tag.
  version: 1.0.0
host: api.pinboard.in
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/update:
    get:
      summary: Update Tag
      description: Returns the most recent time a bookmark was added, updated or deleted.
        Use this before calling posts/all to see if the data has changed since the
        last fetch.
      operationId: posts.update.get
      x-api-path-slug: postsupdate-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/add:
    get:
      summary: Add New Bookmark
      description: Add a new bookmark.
      operationId: posts.add.get
      x-api-path-slug: postsadd-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/delete:
    get:
      summary: Delete a Post
      description: Delete a bookmark.
      operationId: posts.delete.get
      x-api-path-slug: postsdelete-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/get:
    get:
      summary: Get Posts
      description: Returns one or more posts on a single day matching the arguments.
        If no date or url is given, date of most recent bookmark will be used.
      operationId: posts.get.get
      x-api-path-slug: postsget-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/dates:
    get:
      summary: Get Post by Dates
      description: Returns a list of dates with the number of posts at each date.
      operationId: posts.dates.get
      x-api-path-slug: postsdates-get
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Dates
  /posts/recent:
    get:
      summary: Get Recent Posts
      description: Returns a list of the user's most recent posts, filtered by tag.
      operationId: posts.recent.get
      x-api-path-slug: postsrecent-get
      parameters:
      - in: query
        name: count
        description: number of results to return
        type: string
        format: string
      - in: query
        name: tag
        description: filter by up to three tags
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Recent
x-streamrank:
  polling_total_time_average: "0.42"
  polling_size_download_average: "5038.91"
  streaming_total_time_average: "0.22"
  streaming_size_download_average: "2529.82"
  change_yes: "2"
  change_no: "243"
  time_percentage: "48"
  size_percentage: "50"
  change_percentage: "1"
  last_run: "2018-05-06"
  days_run: "1"
  minute_run: "0"
---