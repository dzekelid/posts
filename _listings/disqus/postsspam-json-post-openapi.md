---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Posts Spam
  description: Posts Spam
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
  /posts/list.json:
    get:
      summary: Posts List
      description: Posts List
      operationId: posts-list
      x-api-path-slug: postslist-json-get
      parameters:
      - in: query
        name: category
        description: Defaults to null                         Looks up a category
          by ID
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: end
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: filters
        description: 'Defaults to []                         Valid values are: 1:
          Is_Anonymous 2: Has_Link 3: Has_Low_Rep_Author 4: Has_Bad_Word 5: Is_Flagged
          6: No_Issue 7: Is_Toxic'
        type: string
      - in: query
        name: forum
        description: Defaults to null                         Defaults to all forums
          you moderate
        type: string
      - in: query
        name: include
        description: 'Defaults to [  approved]                         Choices: unapproved,
          approved, spam, deleted, flagged, highlighted'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: offset
        description: 'Defaults to 0                         Deprecated: Please see
          documentation on cursors'
        type: string
      - in: query
        name: order
        description: 'Defaults to desc                         Choices: asc, desc'
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: sortType
        description: 'Defaults to date                         Choices: date, priority'
        type: string
      - in: query
        name: start
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
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
  /posts/listModerationHistory.json:
    get:
      summary: Posts ListModerationHistory
      description: Posts ListModerationHistory
      operationId: posts-listmoderationhistory
      x-api-path-slug: postslistmoderationhistory-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: limit
        description: Defaults to 20
        type: string
      - in: query
        name: post
        description: Looks up a post by ID You must be a moderator on the selected
          post&#39;s forum
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/listPopular.json:
    get:
      summary: Posts ListPopular
      description: Posts ListPopular
      operationId: posts-listpopular
      x-api-path-slug: postslistpopular-json-get
      parameters:
      - in: query
        name: category
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Defaults to null                         Defaults to all forums
          you moderate
        type: string
      - in: query
        name: include
        description: 'Defaults to [  approved]                         Choices: unapproved,
          approved, spam, deleted, flagged, highlighted'
        type: string
      - in: query
        name: interval
        description: 'Defaults to 7d                         Choices: 1h, 6h, 12h,
          1d, 3d, 7d, 30d, 60d, 90d'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: offset
        description: Defaults to 0
        type: string
      - in: query
        name: order
        description: 'Defaults to popular                         Choices: popular,
          best'
        type: string
      - in: query
        name: organization
        description: Defaults to null                         Looks up an organization
          by ID
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
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
  /posts/listReporters.json:
    get:
      summary: Posts ListReporters
      description: Posts ListReporters
      operationId: posts-listreporters
      x-api-path-slug: postslistreporters-json-get
      parameters:
      - in: query
        name: numberPerPost
        description: Defaults to 1
        type: string
      - in: query
        name: posts
        description: Looks up a post by ID You must be a moderator on the selected
          post&#39;s forum
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/remove.json:
    post:
      summary: Posts Remove
      description: Posts Remove
      operationId: posts-remove
      x-api-path-slug: postsremove-json-post
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/report.json:
    post:
      summary: Posts Report
      description: Posts Report
      operationId: posts-report
      x-api-path-slug: postsreport-json-post
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      - in: query
        name: reason
        description: 'Defaults to null                         Valid values are: 0:
          HARASSMENT 1: SPAM 2: INAPPROPRIATE_CONTENT 3: THREAT 4: IMPERSONATION 5:
          PRIVATE_INFORMATION 6: DISAGREE'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/restore.json:
    post:
      summary: Posts Restore
      description: Posts Restore
      operationId: posts-restore
      x-api-path-slug: postsrestore-json-post
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
  /posts/spam.json:
    post:
      summary: Posts Spam
      description: Posts Spam
      operationId: posts-spam
      x-api-path-slug: postsspam-json-post
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID You must be a moderator on the selected
          post&#39;s forum
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
      - Spam
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