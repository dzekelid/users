{
  "info": {
    "name": "PagerDuty Users",
    "_postman_id": "99388078-5766-47b2-8f70-c1c6f8a3696a",
    "description": "Creates a new user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "601c9948-f466-40c0-ad5a-47323c16e7db",
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
          "id": "29cf145e-4a98-4e70-8987-81c5b62a1e9d"
        }
      ]
    }
  ]
}