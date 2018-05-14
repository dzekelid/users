{
  "info": {
    "name": "Particle Delete Orgs Slug Users",
    "_postman_id": "97f7a971-e2d2-4468-b01f-9a1c93503e88",
    "description": "Remove a current team member from your organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "orgs",
      "item": [
        {
          "id": "f78293ff-8724-4345-b93c-31b06101ec1c",
          "name": "deleteOrgsSlugUsersUsername",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.particle.io",
              "path": [
                "v1",
                "orgs/:slug/users/:username"
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
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "slug",
                  "value": "slug",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a current team member from your organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5559bf31-f25d-40c1-a0ae-a7c39f914014"
            }
          ]
        }
      ]
    }
  ]
}