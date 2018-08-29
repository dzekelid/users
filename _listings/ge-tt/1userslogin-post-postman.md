{
  "info": {
    "name": "Ge.tt  REST API Users Login",
    "_postman_id": "5a7e64b4-58fd-447c-b660-c1828adf54b1",
    "description": "The API is based on oauth with an xauth handshake. The request body looks like this:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "cba38d55-53e8-41e3-905f-9e9d11e65c0f",
          "name": "post1FilesSharenameCreate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/create"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To upload files to Ge.tt you must first create the file under a given share. You do that by posting the filename:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3c42f63-2a02-421c-a4b7-2a281f75e61a"
            }
          ]
        },
        {
          "id": "2771bde6-3ff1-46be-a1ac-b9bf80db9f12",
          "name": "get1FilesSharenameFile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the state of a file. This returns the following data:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40d54160-7544-4e47-ae37-faa26fbfd75f"
            }
          ]
        },
        {
          "id": "209aeb69-248b-4eef-84e1-ba4c6b0195b9",
          "name": "get1FilesSharenameFileBlob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to the binary content of the file"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7539f5d0-81e8-4b70-aece-e4222d4fe2c5"
            }
          ]
        },
        {
          "id": "db314dea-f215-4a22-b5d9-6fbdbd163a8d",
          "name": "get1FilesSharenameFileBlobThumb",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob/thumb"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to a thumbnail of the binary file. Currently only available for images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "107e940d-ffd9-4078-92a5-2e89e0e98dba"
            }
          ]
        },
        {
          "id": "133f53fa-5046-4962-821f-0760146dd182",
          "name": "post1FilesSharenameFileDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a file and the binary contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6426bfa-61f4-4285-9cb2-992161545f92"
            }
          ]
        },
        {
          "id": "be66daed-fbfe-4f5a-887f-13dfa9e74cf2",
          "name": "get1FilesSharenameFileUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/upload"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get upload urls to the file. This returns a new PUT and POST url for you to upload the file to.nOBS You can also choose to use the put- or posturl that you were previously given to override the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "612df098-39ec-47e0-a9ec-9726255d272c"
            }
          ]
        }
      ]
    },
    {
      "name": "Shares",
      "item": [
        {
          "id": "8a854ff8-9246-4b36-8cd0-d2cb7e784ab3",
          "name": "get1Shares",
          "request": {
            "url": "http://open.ge.tt/1/1/shares?accesstoken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all your shares and the containing files:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "004eaad9-f37f-4433-b575-ab2a109c013c"
            }
          ]
        },
        {
          "id": "df470a0e-ff6c-415e-8a87-9ab3af1631f7",
          "name": "post1SharesCreate",
          "request": {
            "url": "http://open.ge.tt/1/1/shares/create?accesstoken=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new share. The request body is optional but can look like:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b361ff83-6597-4846-bede-01a8ae24b719"
            }
          ]
        },
        {
          "id": "1e0e51b3-1e77-4d5f-a799-f7c2cc836a14",
          "name": "get1SharesSharename",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename"
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b6e8c94-582d-49df-863c-dd093ca474f2"
            }
          ]
        },
        {
          "id": "3dcb17fa-5814-4578-9c1c-5aaac06d38a0",
          "name": "post1SharesSharenameDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a share and all of its files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "761b178f-aa87-42c9-866c-7bf8015be7bd"
            }
          ]
        },
        {
          "id": "4a04d79a-5dff-43a0-b6e9-5e672bdb2e9c",
          "name": "post1SharesSharenameUpdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename/update"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a share. Currently you can only update the title"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18574842-eedc-4a57-a1dd-b675dd51057a"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "c51ae9c8-af71-4888-83f3-458593a1016f",
          "name": "post1UsersLogin",
          "request": {
            "url": "http://open.ge.tt/1/1/users/login",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The API is based on oauth with an xauth handshake. The request body looks like this:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76a10c86-8169-4bd5-a428-c7a0ec25f952"
            }
          ]
        }
      ]
    }
  ]
}