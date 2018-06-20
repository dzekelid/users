{
  "info": {
    "name": "Viddler  API Users GetSettings",
    "_postman_id": "3cc33d9f-abbf-4144-a270-e5de5c049255",
    "description": "Return account settings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "6ec7c7b6-ee75-48d7-8e64-eabf548a1762",
          "name": "encoding-getsettings",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.encoding.getSettings?sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current encoding options for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cd74fb7-8de5-44c3-a7ee-b9ca458e308d"
            }
          ]
        },
        {
          "id": "9b7e502c-6c59-4421-8839-c63c8347a3c5",
          "name": "users-getsettings",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.users.getSettings?sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return account settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca972e19-7614-439e-be2f-981a08552562"
            }
          ]
        }
      ]
    }
  ]
}