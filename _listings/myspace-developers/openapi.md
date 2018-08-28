swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 1
info:
  title: My Space
  description: create-apps-and-games-within-the-myspace-platform--monetize-through-advertising-and-virtual-goods-
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/statusmoodcomments/{personId}/@self/{statusId}:
    post:
      summary: Post Statusmoodcomments Personid Self Statusid
      description: Posts a comment to a status.
      operationId: 1.0.statusmoodcomments.personId._self.statusId.post
      x-api-path-slug: 1-0statusmoodcommentspersonidselfstatusid-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: filterBy
        description: 'See: http://wiki'
      - in: query
        name: filterOp
        description: 'See: http://wiki'
      - in: query
        name: filterValue
        description: 'See: http://wiki'
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: selector
        description: Indicates which set of individuals to query for activities
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      - in: path
        name: statusId
        description: Specifies which status or mood to post a comment for
      responses:
        200:
          description: OK
      tags:
      - Statusmoodcomments
      - People
      - Self
      - StatusId