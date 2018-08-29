{
  "info": {
    "name": "Learnifier List User Groups.",
    "_postman_id": "2e3bf3ed-f5db-419d-8c94-92b6aa769945",
    "description": "Returns a list of User Groups for the org unit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "0ff25f57-525b-4462-b3d5-b5a958636b2e",
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
              "id": "85021197-c548-4d59-a47e-584a95d4addf"
            }
          ]
        },
        {
          "id": "7a2f5647-27e1-44a5-b79a-15ac0a6b225c",
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
              "id": "b3eaa5e5-e0f4-42a3-87af-0a0434e88d86"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "5fc2b176-b1dd-4626-b734-6ec55a0a413a",
          "name": "orgunits.orgid.usergroups.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "learnifier.com",
              "path": [
                "orgunits/:orgid/usergroups"
              ],
              "variable": [
                {
                  "id": "orgid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of User Groups for the org unit."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d32027aa-ec44-4b40-8636-7f3b31c6fd23"
            }
          ]
        }
      ]
    }
  ]
}