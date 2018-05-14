{
  "info": {
    "name": "Yammer API Retrieve Users By  Messages",
    "_postman_id": "92a80328-e3a4-481d-8799-e7ec08eab3fa",
    "description": "Results will be returned sorted by number of messages, instead of the default behavior of sorting alphabetically.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "c2e8936f-e296-4a7c-9dd3-81e0b2bc2b94",
          "name": "Retrieve Users by # messages_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/users.json"
              ],
              "query": [
                {
                  "key": "sort_by",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Results will be returned sorted by number of messages, instead of the default behavior of sorting alphabetically"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70fd5682-7a80-4635-8d64-df5d670fe842"
            }
          ]
        }
      ]
    }
  ]
}