{
  "info": {
    "name": "Learnifier List Global User Groups.",
    "_postman_id": "e89f91fe-eeb1-4037-8299-12a9fc96c1ae",
    "description": "Returns a list of Global User Groups. Global User Groups are set up for the realm, and will generate groups that can be used on the client level.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "ca07e604-62fe-41af-9d60-05f034df2531",
          "name": "globalusergroups.get",
          "request": {
            "url": "http://learnifier.com/globalusergroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Global User Groups. Global User Groups are set up for the realm, and will generate groups that can be used on the client level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eca05b0-bcad-4a6a-9e65-ab9fc1a2af04"
            }
          ]
        }
      ]
    }
  ]
}