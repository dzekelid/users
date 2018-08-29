{
  "info": {
    "name": "Data.gov API Delete Users User",
    "_postman_id": "49931cad-6fd1-4fa4-9477-8a07d73825c4",
    "description": "Delete a given object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "2c821cfe-68da-4a5a-9ef5-8083cf5a354d",
          "name": "deleteUsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "users/:user/"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a given object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ede2f513-a6e1-4eda-8b70-7cbce178e92e"
            }
          ]
        }
      ]
    }
  ]
}