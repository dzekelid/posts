---
name: Pinboard
x-slug: pinboard
description: Pinboard is a bookmarking website for introverted people in a hurry.
  The focus of the site is less on socializing, and more on speed and utility. Pinboard
  tries to offer useful features without getting in your way. My highest priority
  is keeping your data safe over the long term.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
x-kinRank: "9"
x-alexaRank: "45688"
tags: Posts
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/apis.md
specificationVersion: "0.14"
apis:
- name: Pinboard - Update Tag
  x-api-slug: postsupdate-get
  description: Returns the most recent time a bookmark was added, updated or deleted.
    Use this before calling posts/all to see if the data has changed since the last
    fetch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsupdate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsupdate-get-openapi.md
- name: Pinboard - Add New Bookmark
  x-api-slug: postsadd-get
  description: Add a new bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsadd-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsadd-get-openapi.md
- name: Pinboard - Delete a Post
  x-api-slug: postsdelete-get
  description: Delete a bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsdelete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsdelete-get-openapi.md
- name: Pinboard - Get Posts
  x-api-slug: postsget-get
  description: Returns one or more posts on a single day matching the arguments. If
    no date or url is given, date of most recent bookmark will be used.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsget-get-openapi.md
- name: Pinboard - Get Post by Dates
  x-api-slug: postsdates-get
  description: Returns a list of dates with the number of posts at each date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsdates-get-openapi.md
- name: Pinboard - Get Recent Posts
  x-api-slug: postsrecent-get
  description: Returns a list of the user's most recent posts, filtered by tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsrecent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsrecent-get-openapi.md
- name: Pinboard - Get All Posts
  x-api-slug: postsall-get
  description: Returns all bookmarks in the user's account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postsall-get-openapi.md
- name: Pinboard - Get Popular Tags
  x-api-slug: postssuggest-get
  description: Returns a list of popular tags and recommended tags for a given URL.
    Popular tags are tags used site-wide for the url; recommended tags are drawn from
    the user's own tags.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Bookmarks, Links, My API Stack, Indie EdTech Data Jam, Stack Network, Stack,
    Technology, internet, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postssuggest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/pinboard/postssuggest-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://payrun.api.gallery.streamdata.io
- type: x-api-stack
  url: http://pinboard.stack.network
- type: x-base
  url: https://api.pinboard.in
- type: x-blog
  url: http://www.pinboard.in/blog/
- type: x-blog-rss
  url: https://blog.pinboard.in/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/pinboard
- type: x-crunchbase
  url: http://www.crunchbase.com/company/pinboard
- type: x-developer
  url: https://pinboard.in/api
- type: x-github
  url: https://github.com/pinboard
- type: x-pricing
  url: https://www.pinboard.in/about/
- type: x-privacy
  url: https://www.pinboard.in/privacy/
- type: x-security
  url: https://www.pinboard.in/security/
- type: x-terms-of-service
  url: https://www.pinboard.in/tos/
- type: x-twitter
  url: https://twitter.com/pinboard
- type: x-website
  url: http://pinboard.in
- type: x-website
  url: http://www.pinboard.in
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---