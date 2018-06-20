{
  "info": {
    "name": "PagerDuty Users {user_guid}",
    "_postman_id": "849200b8-d5f9-4268-b254-7d60468734e0",
    "description": "DELETE users user gu",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "eff49713-b97f-49e1-9ba3-9c49f010a0bd",
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
          "id": "70715b76-c1b3-466d-9e63-8d0458f8b541"
        }
      ]
    }
  ]
}