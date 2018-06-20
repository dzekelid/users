{
  "info": {
    "name": "Azure API Management API UserSubscriptions ListByUsers",
    "_postman_id": "24ae4b0f-0901-460e-9c54-747de9b5bb0f",
    "description": "Lists the collection of subscriptions of the specified user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "bead1bcb-aafc-4900-8713-d738061e8527",
          "name": "UserSubscriptions_ListByUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/users/:uid/subscriptions"
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
                  "id": "uid",
                  "value": "uid",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the collection of subscriptions of the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d8fd93d-f4ad-4ed6-b5fb-56e58c913dca"
            }
          ]
        }
      ]
    }
  ]
}