{
  "info": {
    "name": "Data.gov API Delete Users  Followers",
    "_postman_id": "1a8cf98e-098f-4eaa-98ce-aa486a13df90",
    "description": "Unfollow an object given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "b7e5ba92-da3d-417c-8097-12966d4dbf93",
          "name": "deleteUsersFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "users/:id/followers/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unfollow an object given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff5429ab-4f29-418b-b6df-9952354be42c"
            }
          ]
        }
      ]
    }
  ]
}