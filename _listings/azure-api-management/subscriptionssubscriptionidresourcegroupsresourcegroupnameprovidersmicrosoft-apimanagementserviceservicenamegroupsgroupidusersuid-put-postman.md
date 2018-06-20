{
  "info": {
    "name": "Azure API Management API GroupUsers Create",
    "_postman_id": "5fd8f896-fd50-4849-857e-674cb8b5333d",
    "description": "Adds a user to the specified group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group users",
      "item": [
        {
          "id": "7b02d985-33cb-40c8-a368-9e20a1fc6d46",
          "name": "GroupUsers_Create",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/groups/:groupId/users/:uid"
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
                  "id": "groupId",
                  "value": "groupId",
                  "type": "string"
                },
                {
                  "id": "uid",
                  "value": "uid",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a user to the specified group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b1b108e-a0f0-4fed-b983-86522fd7afb7"
            }
          ]
        }
      ]
    }
  ]
}