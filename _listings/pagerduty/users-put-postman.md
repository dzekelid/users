{
  "info": {
    "name": "PagerDuty Users",
    "_postman_id": "1a490f76-f24f-4a88-9e71-fdcf9e9474f4",
    "description": "Updates a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "3daecb7f-3690-48b3-aebc-bcf216251798",
      "name": "list-people-and-integrations-associated-with-a-given-team",
      "request": {
        "url": {
          "protocol": "http",
          "host": "example.com",
          "path": [
            "api",
            "teams/:teamId/people"
          ],
          "variable": [
            {
              "id": "teamId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "List people and integrations associated with a given team."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a6d7a66e-446a-46bf-b187-558b515232fd"
        }
      ]
    }
  ]
}