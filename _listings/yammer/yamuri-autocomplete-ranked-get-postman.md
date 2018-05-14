{
  "info": {
    "name": "Yammer API Get Return Users",
    "_postman_id": "2e144c55-d246-4e60-9503-82e6f121458c",
    "description": "Return typeahead suggestions for the prefix passed",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "73f1d9ad-16d1-4141-8a4d-89bada834105",
          "name": "Get_Return Users, Group, OGs[5]_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/autocomplete/ranked"
              ],
              "query": [
                {
                  "key": "models",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "prefix",
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
            "description": "Return typeahead suggestions for the prefix passed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e3c8a3b-0f9b-4e5f-8155-0d0995354196"
            }
          ]
        }
      ]
    }
  ]
}