---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 1
info:
  title: Blogger
  description: api-for-access-to-the-data-within-blogger-
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /blogger/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}/blogs/{blogId}/posts:
    get:
      summary: Get User Blog Posts
      description: Retrieves a list of post and post user info pairs, possibly filtered.
        The post user info contains per-user information about the post, such as access
        rights, specific to the user.
      operationId: blogger.postUserInfos.list
      x-api-path-slug: usersuseridblogsblogidposts-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch posts from
      - in: query
        name: endDate
        description: Latest post date to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: fetchBodies
        description: Whether the body content of posts is included
      - in: query
        name: labels
        description: Comma-separated list of labels to search for
      - in: query
        name: maxResults
        description: Maximum number of posts to fetch
      - in: query
        name: orderBy
        description: Sort order applied to search results
      - in: query
        name: pageToken
        description: Continuation token if the request is paged
      - in: query
        name: startDate
        description: Earliest post date to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: status
      - in: path
        name: userId
        description: ID of the user for the per-user information to be fetched
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - User Blog Posts
  /users/{userId}/blogs/{blogId}/posts/{postId}:
    get:
      summary: Get User Blog Post
      description: Gets one post and user info pair, by post ID and user ID. The post
        user info contains per-user information about the post, such as access rights,
        specific to the user.
      operationId: blogger.postUserInfos.get
      x-api-path-slug: usersuseridblogsblogidpostspostid-get
      parameters:
      - in: path
        name: blogId
        description: The ID of the blog
      - in: query
        name: maxComments
        description: Maximum number of comments to pull back on a post
      - in: path
        name: postId
        description: The ID of the post to get
      - in: path
        name: userId
        description: ID of the user for the per-user information to be fetched
      responses:
        200:
          description: OK
      tags:
      - User Blog Posts
---