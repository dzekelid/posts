---
name: Tumblr
x-slug: tumblr
description: Tumblr is a place to express yourself, discover yourself, and bond over
  the stuff you love. Its where your interests connect you with your people.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
x-kinRank: "7"
x-alexaRank: "59"
tags: Posts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/apis.md
specificationVersion: "0.14"
apis:
- name: Tumblr Get Blog Base Hostname Adds Type
  x-api-slug: tumblr
  description: Retrieves published posts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
  humanURL: https://www.tumblr.com/
  baseURL: https://api.tumblr.com//v2///blog/{base-hostname}/posts/{type}
  tags: Blog, Base, Hostname, Posts, Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepoststype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepoststype-get-openapi.md
- name: Tumblr Get Blog Base Hostname Adds Queue
  x-api-slug: tumblr
  description: Retrieves queued posts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
  humanURL: https://www.tumblr.com/
  baseURL: https://api.tumblr.com//v2///blog/{base-hostname}/posts/queue
  tags: Blog, Base, Hostname, Posts, Queue
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostsqueue-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostsqueue-get-openapi.md
- name: Tumblr Get Blog Base Hostname Adds Draft
  x-api-slug: tumblr
  description: Retrieves draft posts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
  humanURL: https://www.tumblr.com/
  baseURL: https://api.tumblr.com//v2///blog/{base-hostname}/posts/draft
  tags: Blog, Base, Hostname, Posts, Draft
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostsdraft-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostsdraft-get-openapi.md
- name: Tumblr Get Blog Base Hostname Adds Submission
  x-api-slug: tumblr
  description: Retrieves submission posts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
  humanURL: https://www.tumblr.com/
  baseURL: https://api.tumblr.com//v2///blog/{base-hostname}/posts/submission
  tags: Blog, Base, Hostname, Posts, Submission
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostssubmission-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/blogbasehostnamepostssubmission-get-openapi.md
- name: Tumblr
  x-api-slug: tumblr
  description: Tumblr, is a microblogging platform, emphasizing ease of use, that
    allows users to post text, images, videos, links, quotes and audio to their tumblelog,
    a short-form blog. Users can follow other users, or choose to make their tumblelog
    private.The Tumblr API is currently in its version 2.0, and provides a RESTful
    API that takes advantage of a URI structured including version system(such as
    blog or user), and allows blog owners to use a custom tumblr blog URL or custom
    domains. The API uses OAuth for user authentication and all responses in JSON,
    with JSONP also available. The API provides access to Tumblr Blogs in addition
    to other characteristics like avatars, followers, photos, audio, video and other
    user related information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/265-tumblr.jpg
  humanURL: https://www.tumblr.com/
  baseURL: https://api.tumblr.com//v2/
  tags: Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/tumblr/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/tumblr.json
- type: x-base
  url: http://api.tumblr.com
- type: x-blog
  url: http://staff.tumblr.com/
- type: x-blog-rss
  url: http://staff.tumblr.com/rss
- type: x-crunchbase
  url: http://www.crunchbase.com/company/tumblr
- type: x-crunchbase
  url: https://crunchbase.com/organization/tumblr
- type: x-developer
  url: https://www.tumblr.com/docs/en/api/v2
- type: x-github
  url: https://github.com/tumblr
- type: x-transparency-report
  url: https://www.tumblr.com/transparency
- type: x-twitter
  url: https://twitter.com/tumblr
- type: x-website
  url: https://www.tumblr.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---