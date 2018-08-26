---
swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
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
  /set_block_applied_callback:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts set_block_applied_callback'
      description: set_block_applied_callback
      operationId: set-block-applied-callback-
      x-api-path-slug: set-block-applied-callback-get
      parameters:
      - in: query
        name: cb
        description: callback function
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
      - Block
      - Applied
      - Callback
---