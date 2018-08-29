{
  "info": {
    "name": "Eventbrite Get Users User  Discounts",
    "_postman_id": "795e1759-a141-42ad-8573-a97892d44013",
    "description": "Returns a paginated response of cross_event_discount for the specified user.\nThis operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Discounts",
      "item": [
        {
          "id": "fdd93c5f-17be-40c2-86e3-505725ade4f3",
          "name": "getDiscountsDiscount",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/discounts/:discount_id/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the cross_event_discount with the specified :discount_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b86122d-cd0d-4f71-a1c9-d5686c5d684d"
            }
          ]
        },
        {
          "id": "7d4b7dcf-5791-48ff-b399-abccffa47ea3",
          "name": "postDiscountsDiscount",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/discounts/:discount_id/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the discount with the specified :discount_id. Returns the updated cross_event_discount. The fields sent are the ones that are going to be updated, the fields that are not sent will be unchanged. The same conditions and notes for the discount creation apply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68886627-6d03-4502-a9ff-ece2e9250da9"
            }
          ]
        },
        {
          "id": "28538292-03fd-48c9-9a72-b176d76ce5a4",
          "name": "deleteDiscountsDiscount",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/discounts/:discount_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the cross_event_discount with the specified :discount_id.\nOnly unused discounts can be deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce977b06-16c0-4e19-afd1-fc26d603144a"
            }
          ]
        },
        {
          "id": "daa70227-ab66-4394-95c1-9eada162c965",
          "name": "postDiscounts",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/discounts/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.event_id=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D&discount.ticket_group_id=%7B%7D&discount.type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a discount. Returns the created cross_event_discount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8d1b209-c2e8-4570-9f44-f47082c1723a"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "7df795c7-435d-4b54-82ea-274b4d2635ce",
          "name": "getEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3cf4c46-6ef3-4064-854b-86f3448f0ded"
            }
          ]
        },
        {
          "id": "12873c34-c620-434f-8fc7-bae40ec52206",
          "name": "postEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "857ad702-7f52-42cd-a6e9-342cf5602746"
            }
          ]
        },
        {
          "id": "b631c571-0427-4dd5-8360-24ffbcafc017",
          "name": "getEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdc6c38f-3413-4272-8ce3-26d9b1240df2"
            }
          ]
        },
        {
          "id": "82215a06-954e-4a48-a775-992efac94be0",
          "name": "postEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0635ea95-c244-4337-bd72-af97f7319a08"
            }
          ]
        },
        {
          "id": "7cff12f0-05dd-46c5-bc37-d840efa1d118",
          "name": "deleteEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "819fb1e4-6420-4efa-ae33-828d51d53d0d"
            }
          ]
        },
        {
          "id": "e62e5bcb-275f-48d7-949e-34e090a653ad",
          "name": "getEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1bcafde-6177-4836-8b8b-6e57d39cca73"
            }
          ]
        },
        {
          "id": "613be9a0-a569-49ac-b59e-c991db45868a",
          "name": "postEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0926c94-9ef5-456c-813a-d1d7f87bc03d"
            }
          ]
        },
        {
          "id": "a565dfe1-bf91-4427-a7fa-ae17e7f22646",
          "name": "getEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "408c45e9-aa6b-4001-b061-ea65bdd64de1"
            }
          ]
        },
        {
          "id": "a441c912-c055-4eb8-a47c-59b287c4edb8",
          "name": "postEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c5de456-736d-47ae-90d1-1beb88a71ba7"
            }
          ]
        },
        {
          "id": "edd30637-2016-4773-9d3d-c4b097de40bc",
          "name": "deleteEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55448a20-839d-4150-b8da-00cbe693ec8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "d19acbab-b3b8-45c8-8971-4bbf0fb781c1",
          "name": "getUsersUserDiscounts",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/users/:user_id/discounts/?code=%7B%7D&code_filter=%7B%7D&event_id=%7B%7D&order_by=%7B%7D&page_size=%7B%7D&scope=%7B%7D&ticket_group_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response of cross_event_discount for the specified user.\nThis operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fc9b979-d26c-4d34-a86b-abd57271201c"
            }
          ]
        }
      ]
    }
  ]
}