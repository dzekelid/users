{
  "info": {
    "name": "Data.gov API Add Users  Followers",
    "_postman_id": "38a2c0a5-ea9e-43be-a18d-8ec3f2996157",
    "description": "Follow an user given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "2449ed8a-8667-4a1d-a4af-7ba40f676a74",
          "name": "postUsersFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "users/:id/followers/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Follow an user given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebcdabc2-00a7-4b52-9a9b-a3ab4086c95c"
            }
          ]
        }
      ]
    }
  ]
}