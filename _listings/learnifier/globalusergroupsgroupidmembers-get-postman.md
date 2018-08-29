{
  "info": {
    "name": "Learnifier List of all users in group.",
    "_postman_id": "a1d215c2-25ea-4307-92bf-0700790f2a72",
    "description": "Returns a list of all members in User Groups that are based on the Global Group with this groupid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "84eff2a0-234d-4759-a53c-63415618fb9d",
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
              "id": "4b640033-c036-48e4-80f4-97c5ae4f1029"
            }
          ]
        },
        {
          "id": "33f6bed9-4d6a-49db-af2a-4704fbdd54db",
          "name": "globalusergroups.groupid.members.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "learnifier.com",
              "path": [
                "globalusergroups/:groupid/members"
              ],
              "variable": [
                {
                  "id": "groupid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all members in User Groups that are based on the Global Group with this groupid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "868ecb71-a56d-4ee4-88e7-eed68ac551af"
            }
          ]
        }
      ]
    }
  ]
}