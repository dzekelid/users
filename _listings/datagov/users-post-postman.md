{
  "info": {
    "name": "Data.gov API Add Users",
    "_postman_id": "84180327-6d44-4834-8e9e-ad4a7d5fea12",
    "description": "Create a new object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "245dbca5-6ba9-43d1-96ac-4a3c2f8b514b",
          "name": "postUsers",
          "request": {
            "url": "http://catalog.data.gov/api/3/users/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb2ed37e-4cbd-476f-964a-226ce8963bb1"
            }
          ]
        }
      ]
    }
  ]
}