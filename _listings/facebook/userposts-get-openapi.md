---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get User Adds
  description: The user's posts
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/posts:
    get:
      summary: Get Application Adds
      description: The application's own posts.
      operationId: getApplicationAdds
      x-api-path-slug: applicationposts-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Posts
  /{page}/posts:
    get:
      summary: Get Page Adds
      description: The page's own posts
      operationId: getPageAdds
      x-api-path-slug: pageposts-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Posts
  /{user}/posts:
    get:
      summary: Get User Adds
      description: The user's posts
      operationId: getUserAdds
      x-api-path-slug: userposts-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Posts
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---