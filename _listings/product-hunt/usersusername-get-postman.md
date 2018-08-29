{
  "info": {
    "name": "Product Hunt Users",
    "_postman_id": "80a235b3-f58b-4383-81aa-00bb75015c71",
    "description": "Get Users",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "7aa12fb9-c89b-424b-bde7-93effd7d48d2",
          "name": "users.username.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.producthunt.com",
              "path": [
                "v1",
                "users/:username"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0103522d-fb20-4874-be35-01d96ad2b997"
            }
          ]
        }
      ]
    }
  ]
}