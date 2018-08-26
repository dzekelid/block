---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: 'Steem WARNING: can only be used in Steem node or in scripts set_max_block_age'
  description: set_max_block_age
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_block:
    get:
      summary: get block
      description: get block
      operationId: get-block
      x-api-path-slug: get-block-get
      parameters:
      - in: query
        name: blockNum
        description: get block content/transactions
      responses:
        200:
          description: OK
      tags:
      - Get
      - Block
  /get_block_header:
    get:
      summary: get block header
      description: get block header
      operationId: get-block-header
      x-api-path-slug: get-block-header-get
      parameters:
      - in: query
        name: blockNum
        description: get block header, witness, timestamp
      responses:
        200:
          description: OK
      tags:
      - Get
      - Block
      - Header
  /get_ops_in_block:
    get:
      summary: get_ops_in_block
      description: get_ops_in_block
      operationId: get-ops-in-block
      x-api-path-slug: get-ops-in-block-get
      parameters:
      - in: query
        name: blockNum
        description: block number
      - in: query
        name: onlyVirtual
        description: onlyVirtual
      responses:
        200:
          description: OK
      tags:
      - Get
      - Ops
      - In
      - Block
  /broadcast_block:
    get:
      summary: broadcast_block
      description: broadcast_block
      operationId: broadcast-block
      x-api-path-slug: broadcast-block-get
      parameters:
      - in: query
        name: b
        description: block
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Block
  /set_max_block_age:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts set_max_block_age'
      description: set_max_block_age
      operationId: set-max-block-age
      x-api-path-slug: set-max-block-age-get
      parameters:
      - in: query
        name: maxBlockAge
        description: maxBlockAge
      responses:
        200:
          description: OK
      tags:
      - 'WARNING:'
      - Can
      - Only
      - Be
      - Used
      - In
      - Steem
      - Node
      - In
      - Scripts
      - Set
      - Max
      - Block
      - Age
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