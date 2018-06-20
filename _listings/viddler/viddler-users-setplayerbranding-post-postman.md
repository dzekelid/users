{
  "info": {
    "name": "Viddler  API Users SetPlayerBranding",
    "_postman_id": "4a3ca8cb-f37e-4cb2-b067-c6f94de74091",
    "description": "Sets your player branding options. All options are optional other than your sessionid. Color formats are inu00a0hexadecimalu00a0format with preceding pound sign (IE: #rrggbb)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "8e71eb99-fc56-4b6e-a94e-9e781f15fa36",
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
              "id": "6fdbad6f-690f-4111-ab7c-0fd9025ac6ee"
            }
          ]
        },
        {
          "id": "6b29a824-898f-4dae-92c2-828d06617f57",
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
              "id": "8a9d3cc6-06a4-4c23-a4e9-fc5f5e69d80b"
            }
          ]
        },
        {
          "id": "328606ed-0c4b-46a5-90a1-2ab1bc662714",
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
              "id": "051c5d3c-1e16-4b57-a987-d67f521d2ea7"
            }
          ]
        },
        {
          "id": "b43e188d-75a2-4e30-8323-eaad7695ffbe",
          "name": "users-setplayerbranding",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.users.setPlayerBranding?bclicked=%7B%7D&bhover=%7B%7D&bidle=%7B%7D&control_bar=%7B%7D&enable_stripes=%7B%7D&logo_align=%7B%7D&logo_click_url=%7B%7D&logo_offset_x=%7B%7D&logo_offset_y=%7B%7D&logo_url=%7B%7D&logo_visible=%7B%7D&pclicked=%7B%7D&phover=%7B%7D&pidle=%7B%7D&sessionid=%7B%7D&shade_dark=%7B%7D&simple_color=%7B%7D&timebackground=%7B%7D&timeloaded=%7B%7D&timeplayed=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets your player branding options. All options are optional other than your sessionid. Color formats are inu00a0hexadecimalu00a0format with preceding pound sign (IE: #rrggbb)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fde5bf8b-9792-46af-b0ae-0d0781e9a0da"
            }
          ]
        }
      ]
    }
  ]
}