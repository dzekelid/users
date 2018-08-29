{
  "info": {
    "name": "Azure API Management API Users GenerateSsoUrl",
    "_postman_id": "357b4d8f-c0fa-4fdb-92a7-5d0665c28185",
    "description": "Retrieves a redirection URL containing an authentication token for signing a given user into the developer portal.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "bd81eea3-9808-4d36-bceb-711a322858ee",
          "name": "Users_GenerateSsoUrl",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/users/:uid/generateSsoUrl"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "uid",
                  "value": "uid",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a redirection URL containing an authentication token for signing a given user into the developer portal"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3baf43f-fdc2-414e-b92b-e64fbc4ec6b8"
            }
          ]
        }
      ]
    }
  ]
}