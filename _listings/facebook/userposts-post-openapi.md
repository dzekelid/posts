---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post User Adds
  description: Creates a post on behalf of the user
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
    post:
      summary: Post User Adds
      description: Creates a post on behalf of the user
      operationId: postUserAdds
      x-api-path-slug: userposts-post
      parameters:
      - in: query
        name: actions
        description: Post actions
      - in: query
        name: caption
        description: Post caption
      - in: query
        name: description
        description: Post description
      - in: query
        name: link
        description: Post URL
      - in: query
        name: message
        description: Post message
      - in: query
        name: name
        description: Post name
      - in: query
        name: object_attachment
        description: Facebook ID for an existing picture in the Users photo albums
          to use as the thumbnail image
      - in: query
        name: picture
        description: Post thumbnail image
      - in: query
        name: privacy
        description: Post privacy settings
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