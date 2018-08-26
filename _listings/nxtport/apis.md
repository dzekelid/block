---
name: NxtPort
x-slug: nxtport
description: NxtPort opens the gates to the Port of the future. This project is a
  milestone in the digitalization of logistics and cargo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
x-kinRank: "7"
x-alexaRank: "3933231"
tags: Block
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/nxtport/apis.md
specificationVersion: "0.14"
apis:
- name: T-mining Secure Container Release API (live) - Block
  x-api-slug: apiv1releasesid-delete
  description: |-
    Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
     The following conditions apply for this to work:
    * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
    * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
    * the PickupRight should not yet be assigned (to a driver / skipper)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/nxtport/apiv1releasesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/block/master/_listings/nxtport/apiv1releasesid-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://npr.api.gallery.streamdata.io
- type: x-api-stack
  url: http://nxtport.stack.network
- type: x-email
  url: mail@nxtport.eu
- type: x-email
  url: development@nxtport.eu
- type: x-email
  url: privacy@nxtport.eu
- type: x-github
  url: https://github.com/NxtPort
- type: x-openapi
  url: https://github.com/NxtPort/nxtport.github.io/tree/master/api
- type: x-twitter
  url: https://twitter.com/NxtPortNews
- type: x-website
  url: https://www.nxtport.eu
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---