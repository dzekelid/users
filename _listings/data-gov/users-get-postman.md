{
  "info": {
    "name": "Data.gov API Get Users",
    "_postman_id": "fcf5696e-aac3-4a65-a476-48c97b720229",
    "description": "List all objects",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "b03ecf2f-ffb9-4ac9-8e1a-5cda2560b58f",
          "name": "getUsers",
          "request": {
            "url": "http://catalog.data.gov/api/3/users/?datasets=%7B%7D&facets=%7B%7D&organization=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&reuses=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all objects"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b06e383-e8fd-44a2-8cf3-f61460917f9d"
            }
          ]
        }
      ]
    }
  ]
}