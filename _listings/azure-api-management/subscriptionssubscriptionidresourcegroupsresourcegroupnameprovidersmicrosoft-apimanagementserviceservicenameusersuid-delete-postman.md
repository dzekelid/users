{
  "info": {
    "name": "Azure API Management API Users Delete",
    "_postman_id": "71524e08-f649-4fce-b035-6a6c9cc6bba3",
    "description": "Deletes specific user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "b700812b-1a51-4daa-a9c0-4d095aebfc16",
          "name": "Users_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/users/:uid"
              ],
              "query": [
                {
                  "key": "deleteSubscriptions",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "method": "DELETE",
            "header": [
              {
                "key": "If-Match",
                "value": "{}",
                "description": "The entity state (Etag) version of the user to delete",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes specific user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "148f0298-f5f5-4d47-831f-4c2a3a1ca691"
            }
          ]
        }
      ]
    }
  ]
}