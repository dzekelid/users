{
  "info": {
    "name": "Data.gov API Get Users Suggest",
    "_postman_id": "1c8a0569-93d7-457b-a43e-153f919ab493",
    "description": "Suggest users",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "717c527a-cb47-4565-8684-b14921d08076",
          "name": "getUsersSuggest",
          "request": {
            "url": "http://catalog.data.gov/api/3/users/suggest/?q=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suggest users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "130e7b00-e2c0-4baf-98a3-38a2864bbef4"
            }
          ]
        }
      ]
    }
  ]
}