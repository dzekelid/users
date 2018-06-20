{
  "info": {
    "name": "Icon Finder Get user details",
    "_postman_id": "39d9f2d5-958c-4593-a7e2-09cf33e06425",
    "description": "Get details about a specific user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Authors",
      "item": [
        {
          "id": "9b92686f-db76-4f0b-96c8-1cd93bf70d2b",
          "name": "getAuthorsAuthor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "authors/:authorID"
              ],
              "query": [
                {
                  "key": "authors",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "authorID",
                  "value": "authorID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific author identified by a unique ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccd582ac-ee88-4b9e-883e-5ad44e351f8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "a0a0e653-8440-40f9-8ce3-858313e47a79",
          "name": "getCategories",
          "request": {
            "url": "http://api.iconfinder.com/v2/categories?after=%7B%7D&count=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all categories sorted ascendingly by their identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e20c492d-e39a-4180-badc-6b27bb0099bb"
            }
          ]
        },
        {
          "id": "a99e6750-26e8-427f-a5d8-3edc2cac830a",
          "name": "getV2CategoriesCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "v2/categories/:categoryID"
              ],
              "variable": [
                {
                  "id": "categoryID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific category identified by its identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f4fb6d8-9374-41d0-95e9-a1a2a9c641ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Icons",
      "item": [
        {
          "id": "a4ee0a13-3aa9-4f3e-bda0-6d9cee4cf4a4",
          "name": "getIconsSearch",
          "request": {
            "url": "http://api.iconfinder.com/v2/icons/search?category=%7B%7D&count=%7B%7D&license=%7B%7D&maximum_size=%7B%7D&minimum_size=%7B%7D&offset=%7B%7D&premium=%7B%7D&query=%7B%7D&style=%7B%7D&vector=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search through icons by various criteria. The returned list of icons is ordered descendingly by popularit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cab629cb-b743-4e8c-962d-bccded0d69f8"
            }
          ]
        },
        {
          "id": "99d882f6-31ba-4c8a-aee1-8ce50166dd90",
          "name": "getV2IconsIcon",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "v2/icons/:iconID"
              ],
              "variable": [
                {
                  "id": "iconID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific ico"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b26f9540-0132-413f-8cd7-1020d5c8b455"
            }
          ]
        },
        {
          "id": "b29feb9c-38f3-48fc-8ede-1027d0f9b757",
          "name": "getV2IconsetsIconIcons",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "v2/iconsets/:iconID/icons"
              ],
              "query": [
                {
                  "key": "after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "List all icons in an icon set",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "iconID",
                  "value": "iconID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a list of all icons in an icon set sorted descendingly by the popularity of the icons.List all icons in an icon set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcb86749-a0fc-4b77-9a7b-a499320b9357"
            }
          ]
        }
      ]
    },
    {
      "name": "Licenses",
      "item": [
        {
          "id": "42a3ce13-3ff9-41a7-a650-37edfe9403db",
          "name": "getLicensesLicense",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "licenses/:licenseID"
              ],
              "variable": [
                {
                  "id": "licenseID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific license by its unique ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c5ea97-df3f-4736-847a-9fb2876d83c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Styles",
      "item": [
        {
          "id": "2904c7da-1f67-4c06-88ad-0018ac85a5d6",
          "name": "getStylesStyle",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "styles/:styleID"
              ],
              "variable": [
                {
                  "id": "styleID",
                  "value": "styleID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific style identified by its identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36137d8-9eda-4faf-8fb4-74650f64032c"
            }
          ]
        },
        {
          "id": "fe0ac11c-45b3-48d7-acfa-48c5c661bda3",
          "name": "getV2Styles",
          "request": {
            "url": "http://api.iconfinder.com/v2/v2/styles?after=%7B%7D&count=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all styles sorted ascendingly by their identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0bfef01-b34f-442e-b780-cb4a9243d18c"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "68cc6dc7-a0a3-4f9a-8b5a-85565058ed32",
          "name": "getUser",
          "request": {
            "url": "http://api.iconfinder.com/v2/user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ee15367-cbc1-41c9-83ff-c859f5866d3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "d4345e3e-68b8-47fb-b558-2fb3c966c298",
          "name": "getGetV2UsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "GET /v2/users/:userID"
              ],
              "variable": [
                {
                  "id": "userID",
                  "value": "userID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b53c8f23-ef44-402d-9bc9-b3585b23ae51"
            }
          ]
        }
      ]
    }
  ]
}