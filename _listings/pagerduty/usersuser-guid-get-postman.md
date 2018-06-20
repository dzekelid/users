{
  "info": {
    "name": "PagerDuty Users {user_guid}",
    "_postman_id": "10300444-ea3e-402d-bbe7-ad205405428d",
    "description": "Returns customer's user by user GUID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "e825a902-b00d-4cb3-80b5-a07f1eb58cba",
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
          "id": "68a7132c-e4c2-4286-b85b-cca538b364ae"
        }
      ]
    }
  ]
}