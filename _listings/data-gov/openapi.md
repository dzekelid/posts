swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
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
    get:
      summary: Get Post
      description: Get a given post
      operationId: getPostsPost
      x-api-path-slug: postspost-get
      parameters:
      - in: path
        name: post
        description: The post ID or slug
      responses:
        200:
          description: OK
      tags:
      - Posts
    put:
      summary: Update Post
      description: Update a given post
      operationId: putPostsPost
      x-api-path-slug: postspost-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: post
        description: The post ID or slug
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{post}/image:
    post:
      summary: Add Post Image
      description: Upload a new image
      operationId: postPostsPostImage
      x-api-path-slug: postspostimage-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: post
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Images
    put:
      summary: Update Post Image
      description: Set the image BBox
      operationId: putPostsPostImage
      x-api-path-slug: postspostimage-put
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: post
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Images