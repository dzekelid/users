{
  "info": {
    "name": "Data.gov API Get Users  Followers",
    "_postman_id": "ad7929d3-4dcc-487c-a1bc-e7a3e1c335d9",
    "description": "List all followers for a given object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "377590bc-b907-4412-8b74-28e4fef6cc2a",
          "name": "getUsersFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "users/:id/followers/"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
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
            "description": "List all followers for a given object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4773ab48-8435-402e-9fc7-d5872964df0e"
            }
          ]
        }
      ]
    }
  ]
}