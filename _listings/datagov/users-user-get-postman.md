{
  "info": {
    "name": "Data.gov API Get Users User",
    "_postman_id": "b45a1607-b5fd-4d1c-83ab-79c3a7dbdcf6",
    "description": "Get a given object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "0639503b-10e7-4b14-918f-b9d4bd2b7bca",
          "name": "getUsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "users/:user/"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a given object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ef6f250-b5e3-433e-b8be-1f1d4faed0cb"
            }
          ]
        }
      ]
    }
  ]
}