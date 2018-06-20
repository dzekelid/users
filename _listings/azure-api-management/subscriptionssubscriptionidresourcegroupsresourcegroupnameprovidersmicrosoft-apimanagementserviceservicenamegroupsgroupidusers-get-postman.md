{
  "info": {
    "name": "Azure API Management API GroupUsers ListByGroups",
    "_postman_id": "032462e9-3216-4141-9651-3f3894531f7a",
    "description": "Lists a collection of the members of the group, specified by its identifier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group users",
      "item": [
        {
          "id": "04e7de79-e413-4e9f-9e3d-2e1e240596b9",
          "name": "GroupUsers_ListByGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/groups/:groupId/users"
              ],
              "query": [
                {
                  "key": "$filter",
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
                  "id": "groupId",
                  "value": "groupId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a collection of the members of the group, specified by its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e6dd0e9-d27c-4670-b4f8-f92fc46c6499"
            }
          ]
        }
      ]
    }
  ]
}