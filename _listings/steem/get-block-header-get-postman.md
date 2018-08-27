{
  "info": {
    "name": "Steem get block header",
    "_postman_id": "a7b1f29a-c93d-48ed-b9dd-93a4652f70aa",
    "description": "get block header",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "517c4e1d-fe4c-4bd0-b849-1dd28a6cc7c2",
          "name": "get-block",
          "request": {
            "url": "http://api.steemjs.com/get_block?blockNum=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83d9e899-cc3c-48b8-8ce4-c7efcd4f03c2"
            }
          ]
        },
        {
          "id": "6749367f-fb28-4343-b8c5-2cd344a718cb",
          "name": "get-block-header",
          "request": {
            "url": "http://api.steemjs.com/get_block_header?blockNum=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get block header"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47ed2882-d938-468a-aea1-1c2aed768417"
            }
          ]
        }
      ]
    }
  ]
}