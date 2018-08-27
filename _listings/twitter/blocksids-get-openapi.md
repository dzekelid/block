---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Block Users
  description: returns array of numeric user ids of blocked users
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blocks/list:
    get:
      summary: Block List
      description: disallows retweets and device notifications from a user
      operationId: disallows-retweets-and-device-notifications-from-a-user
      x-api-path-slug: blockslist-get
      parameters:
      - in: query
        name: cursor
        description: breaks block of user to be broken up into pages
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: skip_status
        description: whether or not to include statuses in response
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /blocks/ids:
    get:
      summary: Block Users
      description: returns array of numeric user ids of blocked users
      operationId: returns-array-of-numeric-user-ids-of-blocked-users
      x-api-path-slug: blocksids-get
      parameters:
      - in: query
        name: cursor
        description: breaks up block of user IDs into pages
      - in: query
        name: stringify_ids
        description: returns array of numeric IDs as string IDs
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
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