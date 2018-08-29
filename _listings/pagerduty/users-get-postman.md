{
  "info": {
    "name": "PagerDuty Users",
    "_postman_id": "f02db1e0-6902-43fa-a0aa-d87fad082bd0",
    "description": "Returns all customer's users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "42163c22-f24f-496b-972d-4581e9c66748",
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
          "id": "f40bea6a-0b68-4810-94b9-2760d045843d"
        }
      ]
    }
  ]
}