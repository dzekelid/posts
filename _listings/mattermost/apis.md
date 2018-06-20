---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Posts
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Get a channels pinned posts
  x-api-slug: mattermost-api
  description: Get a list of pinned posts for channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//channels/{channel_id}/pinned
  tags: Channels,Pinned,Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/channelschannel-idpinned-get-openapi.md
- name: Mattermost API Get a list of flagged posts
  x-api-slug: mattermost-api
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/posts/flagged
  tags: List,Of,Flagged,Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/usersuser-idpostsflagged-get-openapi.md
- name: Mattermost API Get posts for a channel
  x-api-slug: mattermost-api
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//channels/{channel_id}/posts
  tags: Postsa,Channel
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Search for team posts
  x-api-slug: mattermost-api
  description: |-
    Search posts in the team and from the provided terms string.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/posts/search
  tags: Searchteam,Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/teamsteam-idpostssearch-post-openapi.md
- name: Mattermost API
  x-api-slug: mattermost-api
  description: Open source, private cloud Slack-alternative, Workplace messaging for
    web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
    configurable, and scalable from teams to the enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/posts/master/_listings/mattermost/openapi.md
x-common:
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---