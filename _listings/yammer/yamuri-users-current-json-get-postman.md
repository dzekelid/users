{
  "info": {
    "name": "Yammer API Get Current User",
    "_postman_id": "2f9a8002-5955-4c57-891a-72621a0e7901",
    "description": "View data about the current user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "1c11e679-0d34-42e1-9442-d3a4a5ee4acc",
          "name": "Get_Current User_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/users/current.json"
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
            "description": "View data about the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acf06baa-2fcb-4131-9998-7fcc2dc75785"
            }
          ]
        }
      ]
    }
  ]
}