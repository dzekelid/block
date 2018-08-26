---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 1
info:
  title: Twitter
  description: the-twitter-api-gives-you-programmatic-control-over-any-twitter-account-and-most-aspect-of-the-platform--allowing-developers-to-build-social-applications-that-use-the-platform-and-automate-interactions-between-users-
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
  /blocks/create:
    post:
      summary: Block User
      description: blocks the specified user
      operationId: blocks-the-specified-user
      x-api-path-slug: blockscreate-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be blocked
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to be blocked
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /blocks/destroy:
    post:
      summary: Unblock User
      description: un-blocks the specified user
      operationId: unblocks-the-specified-user
      x-api-path-slug: blocksdestroy-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be un-blocked
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to be un-blocked
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
---