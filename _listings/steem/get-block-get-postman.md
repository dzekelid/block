{
  "info": {
    "name": "Steem get block",
    "_postman_id": "ede718c9-86ab-421c-bba1-aeb31c70a353",
    "description": "get block",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "86d4ed63-b7ee-46b5-a606-85d1990b42f5",
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
              "id": "dd3a8fdf-c5c1-4ae5-9e16-5e0441892c22"
            }
          ]
        }
      ]
    }
  ]
}