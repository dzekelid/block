---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 1
info:
  title: Neblio REST API Suite
  description: apis-for-interacting-with-ntp1-tokens--the-neblio-blockchain
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: getBlock
      x-api-path-slug: insblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /ins/block-index/{blockindex}:
    get:
      summary: Returns block hash of block
      description: Returns the block hash of a block at a given block index
      operationId: getBlockIndex
      x-api-path-slug: insblockindexblockindex-get
      parameters:
      - in: path
        name: blockindex
        description: Block Index
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Block
      - Hash
      - Of
      - Block
  /ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: getTxs
      x-api-path-slug: instxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /testnet/ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: testnet_getBlock
      x-api-path-slug: testnetinsblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /testnet/ins/block-index/{blockindex}:
    get:
      summary: Returns block hash of block
      description: Returns the block hash of a block at a given block index
      operationId: testnet_getBlockIndex
      x-api-path-slug: testnetinsblockindexblockindex-get
      parameters:
      - in: path
        name: blockindex
        description: Block Index
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Block
      - Hash
      - Of
      - Block
  /testnet/ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: testnet_getTxs
      x-api-path-slug: testnetinstxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
---