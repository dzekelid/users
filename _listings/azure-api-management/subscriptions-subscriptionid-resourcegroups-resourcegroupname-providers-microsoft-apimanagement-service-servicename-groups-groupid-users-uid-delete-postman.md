{
  "info": {
    "name": "Azure API Management API GroupUsers Delete",
    "_postman_id": "98e554e6-be4f-4ab9-b076-145800533d3c",
    "description": "Remove existing user from existing group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group users",
      "item": [
        {
          "id": "f40b5931-8da3-4273-a843-6accb3664279",
          "name": "GroupUsers_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove existing user from existing group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64f0d1a8-38b4-4f57-86fe-40e85048e6a1"
            }
          ]
        }
      ]
    }
  ]
}