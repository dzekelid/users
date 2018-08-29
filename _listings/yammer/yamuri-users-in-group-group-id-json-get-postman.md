{
  "info": {
    "name": "Yammer API Get Users In A Group",
    "_postman_id": "951f1fd3-418c-4c1c-946e-9516d241ef89",
    "description": "Users in a group. Supports the page parameter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "f3f3ddba-d603-4c46-805d-21bcc39c305f",
          "name": "Get_Users in a Group_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/users/in_group/:group_id.json"
              ],
              "variable": [
                {
                  "id": "group_id",
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
            "description": " Users in a group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3ab2692-8656-450b-b6a1-1aa524fb5023"
            }
          ]
        }
      ]
    }
  ]
}