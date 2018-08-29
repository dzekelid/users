{
  "info": {
    "name": "Viddler  API Users SetProfile",
    "_postman_id": "fb8aff12-a4f5-4813-9190-834c88d44247",
    "description": "Update your profile information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "eabfd55e-7fea-4490-a10f-4e61bae5a277",
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
              "id": "a7da19e0-7ea6-45b6-9d85-bbcbf5d0fe06"
            }
          ]
        },
        {
          "id": "fe94e811-af2b-4bdd-a90c-94f5d63deb49",
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
              "id": "e9ceaa73-1c52-41f7-be93-d06c82b7a5ec"
            }
          ]
        },
        {
          "id": "cefe4151-569a-4887-8ea3-69467d6f1013",
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
              "id": "3bffa7a3-498b-48ce-88a7-41cc1a69691f"
            }
          ]
        },
        {
          "id": "197c3ac3-7e00-4083-9e3d-4fad49260685",
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
              "id": "f3792d11-e368-4faa-a354-ff4af814ffd0"
            }
          ]
        },
        {
          "id": "07d0c7ce-1abc-47fd-be66-5ffd6493b9aa",
          "name": "users-setprofile",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.users.setProfile?avatar_url=%7B%7D&homepage=%7B%7D&sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Update your profile information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3db57bcb-785f-44b7-a405-df8af708dac9"
            }
          ]
        }
      ]
    }
  ]
}