{
  "info": {
    "name": "Viddler  API Users GetProfile",
    "_postman_id": "f5d09038-1c50-4163-a21b-b3068f5471d7",
    "description": "Get the public information for a profile. Can only get profile information for public profiles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "f96070b4-a738-4a3d-a3ba-973580abe6fb",
          "name": "users-getplayerbranding",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.users.getPlayerBranding?sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns your player branding configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71807b33-0b05-4f21-a61a-c12c8f2862bb"
            }
          ]
        },
        {
          "id": "2a190ab3-e781-418e-b73b-dca2f5d26dca",
          "name": "users-getprofile",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.users.getProfile?sessionid=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the public information for a profile. Can only get profile information for public profiles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce05e1de-895b-43d4-afbb-5d1a8d2427a7"
            }
          ]
        }
      ]
    }
  ]
}