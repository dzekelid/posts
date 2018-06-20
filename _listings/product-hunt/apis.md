---
name: Product Hunt
x-slug: product-hunt
description: Product Hunt (YC S14) surfaces the best new products, every day. Its
  a place for product-loving enthusiasts to share and geek out about the latest mobile
  apps, websites, hardware projects, and tech creations.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/product-hunt-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Posts
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/product-hunt/apis.md
specificationVersion: "0.14"
apis:
- name: Product Hunt Posts
  x-api-slug: product-hunt
  description: Get posts by category.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/product-hunt-logo.png
  humanURL: https://www.producthunt.com/
  baseURL: https://api.producthunt.com//v1//categories/{category}/posts
  tags: Posts,Products,Services
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/product-hunt/categoriescategoryposts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/product-hunt/categoriescategoryposts-get-openapi.md
- name: Product Hunt
  x-api-slug: product-hunt
  description: Product Hunt (YC S14) surfaces the best new products, every day. Its
    a place for product-loving enthusiasts to share and geek out about the latest
    mobile apps, websites, hardware projects, and tech creations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/product-hunt-logo.png
  humanURL: https://www.producthunt.com/
  baseURL: https://api.producthunt.com//v1
  tags: Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/product-hunt/openapi.md
x-common:
- type: x-blog
  url: https://blog.producthunt.com/
- type: x-blog-rss
  url: https://blog.producthunt.com/feed
- type: x-github
  url: https://github.com/producthunt
- type: x-twitter
  url: https://twitter.com/producthunt
- type: x-website
  url: https://www.producthunt.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---