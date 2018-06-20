---
swagger: "2.0"
x-collection-name: Pinboard
x-complete: 0
info:
  title: Pinboard Get Popular Tags
  description: Returns a list of popular tags and recommended tags for a given URL.
    Popular tags are tags used site-wide for the url; recommended tags are drawn from
    the user's own tags.
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
  /posts/all:
    get:
      summary: Get All Posts
      description: Returns all bookmarks in the user's account.
      operationId: posts.all.get
      x-api-path-slug: postsall-get
      parameters:
      - in: query
        name: fromdt
        description: return only bookmarks created after this time
        type: string
        format: string
      - in: query
        name: meta
        description: include a change detection signature for each bookmark
        type: string
        format: string
      - in: query
        name: results
        description: number of results to return
        type: string
        format: string
      - in: query
        name: start
        description: offset value (default is 0)
        type: string
        format: string
      - in: query
        name: tag
        description: filter by up to three tags
        type: string
        format: string
      - in: query
        name: todt
        description: eturn only bookmarks created before this time
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/suggest:
    get:
      summary: Get Popular Tags
      description: Returns a list of popular tags and recommended tags for a given
        URL. Popular tags are tags used site-wide for the url; recommended tags are
        drawn from the user's own tags.
      operationId: posts.suggest.get
      x-api-path-slug: postssuggest-get
      parameters:
      - in: query
        name: format
        description: the format to return
        type: string
        format: string
      - in: query
        name: url
        description: url to suggest from
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Suggest
x-streamrank:
  polling_total_time_average: "0.42"
  polling_size_download_average: "248.8"
  streaming_total_time_average: "0.27"
  streaming_size_download_average: "143.6"
  change_yes: "4"
  change_no: "1"
  time_percentage: "35"
  size_percentage: "42"
  change_percentage: "80"
  last_run: "2018-05-05"
  days_run: "0"
  minute_run: "0"
---