---
name: MasterCard
x-slug: mastercard
description: Mastercard is a leading global payments & technology company that connects
  consumers, businesses, merchants, issuers & governments around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
x-kinRank: "9"
x-alexaRank: "48280"
tags: Block
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/mastercard/apis.md
specificationVersion: "0.14"
apis:
- name: MasterCard - Get Block
  x-api-slug: block-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/mastercard/block-get-openapi.md
- name: MasterCard - Get Block Key
  x-api-slug: blockkey-get
  description: |-
    A specific block may be retrieved by its hash key. This is useful when
    navigating the chain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/mastercard/blockkey-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://mapquest.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mastercard.stack.network
- type: x-base
  url: https://api.simplify.com
- type: x-blog
  url: https://developer.mastercard.com/portal/display/blogs/Developer+Blogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/mastercard
- type: x-crunchbase
  url: http://www.crunchbase.com/company/mastercard
- type: x-github
  url: https://github.com/MasterCard
- type: x-website
  url: https://developer.mastercard.com/
- type: x-twitter
  url: https://twitter.com/AskMastercard
- type: x-twitter
  url: https://twitter.com/MasterCardDev
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---