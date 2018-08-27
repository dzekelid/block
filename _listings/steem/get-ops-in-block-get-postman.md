{
  "info": {
    "name": "Steem get_ops_in_block",
    "_postman_id": "e4c1c811-afee-40a4-bee2-fb87ea58567a",
    "description": "get_ops_in_block",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "b8bbef75-4c75-4496-bb28-f3347244a964",
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
              "id": "0c08f96a-635d-475b-b3cc-c132ededd1f8"
            }
          ]
        },
        {
          "id": "062a7f22-e899-4c72-a3f0-17a8c2c50d03",
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
              "id": "499d884b-464c-4c34-948b-d02f95464fa0"
            }
          ]
        },
        {
          "id": "b5b54961-168d-45c9-bdbb-528cd21e8073",
          "name": "get-ops-in-block",
          "request": {
            "url": "http://api.steemjs.com/get_ops_in_block?blockNum=%7B%7D&onlyVirtual=%7B%7D",
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
            "description": "get_ops_in_block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba2d44df-1edb-4884-b7f6-152cab12e725"
            }
          ]
        }
      ]
    }
  ]
}