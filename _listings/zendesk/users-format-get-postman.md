{
  "info": {
    "name": "Sales Force Desk API Get Users",
    "_postman_id": "f614622c-bc75-46ba-9244-4c5f84a3ce74",
    "description": "Get users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "35bc6dda-a5a5-4fa3-aa02-a9ebc95b194f",
          "name": "get-users",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/users.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f0b8b62-ec37-4146-b51f-2e0c6c315a90"
            }
          ]
        }
      ]
    }
  ]
}