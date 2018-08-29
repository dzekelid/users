{
  "info": {
    "name": "Azure DevTest Labs API Users Delete",
    "_postman_id": "d5b9a2a4-3e45-43ef-bf99-572355c32721",
    "description": "Delete user profile. This operation can take a while to complete.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "b4038ce8-856d-463f-a6ec-46674186f949",
          "name": "Users_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/users/:name"
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
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a9c90eb-d828-4a14-be47-2b1c7dc8add0"
            }
          ]
        }
      ]
    }
  ]
}