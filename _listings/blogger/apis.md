---
name: Blogger
x-slug: blogger
description: Blogger is a blog-publishing service that allows multi-user blogs with
  time-stamped entries. It was developed by Pyra Labs, which was bought by Google
  in 2003. Generally, the blogs are hosted by Google at a subdomain of blogspot.com.
  Blogs can also be hosted in the registered custom domain of the blogger (like www.example.com).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Posts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/blogger/apis.md
specificationVersion: "0.14"
apis:
- name: Blogger API Get User Blog Posts
  x-api-slug: blogger-api
  description: Retrieves a list of post and post user info pairs, possibly filtered.
    The post user info contains per-user information about the post, such as access
    rights, specific to the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs/{blogId}/posts
  tags: User Blog Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/blogger/usersuseridblogsblogidposts-get-openapi.md
- name: Blogger API Get User Blog Post
  x-api-slug: blogger-api
  description: Gets one post and user info pair, by post ID and user ID. The post
    user info contains per-user information about the post, such as access rights,
    specific to the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs/{blogId}/posts/{postId}
  tags: User Blog Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/blogger/usersuseridblogsblogidpostspostid-get-openapi.md
- name: Blogger API
  x-api-slug: blogger-api
  description: The Blogger API v3 allows client applications to view and update Blogger
    content. Your client application can use Blogger API v3 to create new blog posts,
    edit or delete existing posts, and query for posts that match particular criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/blogger/openapi.md
x-common:
- type: x-blog
  url: https://blogger.googleblog.com/
- type: x-website
  url: https://www.blogger.com
- type: x-blog-rss
  url: http://buzz.blogger.com/atom.xml
- type: x-developer
  url: https://developers.google.com/blogger/
- type: x-twitter
  url: https://twitter.com/Blogger
- type: x-getting-started
  url: https://developers.google.com/blogger/docs/3.0/getting_started
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---