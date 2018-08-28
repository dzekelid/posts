swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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
  /teams/{team_id}/posts/search:
    post:
      summary: Search for team posts
      description: |-
        Search posts in the team and from the provided terms string.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: search-posts-in-the-team-and-from-the-provided-terms-string-permissionsmust-be-authenticated-and-hav
      x-api-path-slug: teamsteam-idpostssearch-post
      parameters:
      - in: body
        name: body
        description: The search terms and logic to use in the search
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Searchteam
      - Posts