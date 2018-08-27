swagger: "2.0"
x-collection-name: MasterCard
x-complete: 1
info:
  title: MasterCard
  description: as-a-technology-company-in-the-global-payments-business-we-operate-the-worlds-fastest-payments-processing-network-connecting-consumers-financial-institutions-merchants-governments-and-businesses-in-more-than-210-countries-and-territories--mastercards-products-and-solutions-make-everyday-commerce-activities--such-as-shopping-traveling-running-a-business-and-managing-finances--easier-more-secure-and-more-efficient-for-everyone-
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /block:
    get:
      summary: Get Block
      description: |-
        By default, this call returns the last confirmed block, since the `from`
        and `to` parameters will both default to the last confirmed slot number.
        To get a range of blocks, use the `from` and `to` parameters. Specifying
        only the `from` parameter will get a range of blocks up to the current slot.
        Note that this also means that specifying `to` without `from` will result
        in an error since that will mean a negative range.

        For each returned item, the data will contain header information from
        the block binary, and references to the block entries via the merkle roots.

        Note that the maximum range request allowed is 600 entries.
      operationId: getBlock
      x-api-path-slug: block-get
      parameters:
      - in: query
        name: from
        description: Specify the starting slot to return
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      - in: query
        name: to
        description: Specify the last slot to return
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Block
  /block/{key}:
    get:
      summary: Get Block Key
      description: |-
        A specific block may be retrieved by its hash key. This is useful when
        navigating the chain.
      operationId: getBlockKey
      x-api-path-slug: blockkey-get
      parameters:
      - in: path
        name: key
        description: The hash key of the block to retrieve
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Block
      - Key