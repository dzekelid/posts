---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get a list of flagged posts
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/{channel_id}/pinned:
    get:
      summary: Get a channels pinned posts
      description: Get a list of pinned posts for channel.
      operationId: get-a-list-of-pinned-posts-for-channel
      x-api-path-slug: channelschannel-idpinned-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channels
      - Pinned
      - Posts
  /users/{user_id}/posts/flagged:
    get:
      summary: Get a list of flagged posts
      description: |-
        Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
        ##### Permissions
        Must be user or have `manage_system` permission.
      operationId: get-a-page-of-flagged-posts-of-a-user-provided-user-id-string-selects-from-a-channel-team-or-all-fla
      x-api-path-slug: usersuser-idpostsflagged-get
      parameters:
      - in: query
        name: channel_id
        description: Channel ID
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of posts per page
      - in: query
        name: team_id
        description: Team ID
      - in: path
        name: user_id
        description: ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Flagged
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