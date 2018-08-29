{
  "info": {
    "name": "Yammer API Get Specific User By ID",
    "_postman_id": "048471d8-f7fc-4677-bbc5-0216c3b5f28e",
    "description": "View data about a user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "7579d1d9-d7dd-477b-9475-af97453e3ff0",
          "name": "Get_Specific User by ID_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/users/:user_id.json"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View data about a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5469a937-99bf-4f37-ae19-5bf751faa251"
            }
          ]
        }
      ]
    }
  ]
}