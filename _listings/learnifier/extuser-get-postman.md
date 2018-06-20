{
  "info": {
    "name": "Learnifier Gets a user by external id",
    "_postman_id": "657a3a57-8bb3-4582-b66b-de6dba6c660a",
    "description": "Gets a user by external id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "a95a98a5-6c54-4a12-ae64-ff53e311a397",
          "name": "extuser.get",
          "request": {
            "url": "http://learnifier.com/extuser?extid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a user by external id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c278ce8-bc24-4f36-89d1-572978463b33"
            }
          ]
        }
      ]
    }
  ]
}