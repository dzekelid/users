{
  "info": {
    "name": "Yammer API Get Specific User By Email",
    "_postman_id": "16ec5965-5d30-404d-aefb-ab3b52dd314a",
    "description": "View data about a user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "525b595a-c37b-41a3-8728-33d1185b0edc",
          "name": "Get_Specific User by Email_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/users/by_email.json"
              ],
              "query": [
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
              "id": "322404c6-6427-4d15-b160-81e1c8d39fac"
            }
          ]
        }
      ]
    }
  ]
}