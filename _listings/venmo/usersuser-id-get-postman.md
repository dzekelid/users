{
  "info": {
    "name": "Venmo API Get Users User",
    "_postman_id": "1cc0d6e4-9d8b-4419-bf13-d16b48e85878",
    "description": "Get users user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "44ddcdb4-7724-400a-9601-9cd357932d12",
          "name": "getUsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.venmo.com",
              "path": [
                "v1",
                "users/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get users user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8033f266-b0ae-4f6d-a2d8-5d5f50b8f334"
            }
          ]
        }
      ]
    }
  ]
}