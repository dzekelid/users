{
  "info": {
    "name": "Sales Force Desk API Get User",
    "_postman_id": "45713b2d-df33-47e5-95e8-bb24404592a1",
    "description": "Get user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "9fe2bd6a-3e0e-4e72-8314-c129e2f64ead",
          "name": "get-users",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/users.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b77aa8e8-6158-4d15-8362-1985165782e0"
            }
          ]
        },
        {
          "id": "8fd4cbef-1565-4fb2-895a-465bdabb7017",
          "name": "get-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "users/:id.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b844b30-c78e-4e2f-97c7-20a4329f639b"
            }
          ]
        }
      ]
    }
  ]
}