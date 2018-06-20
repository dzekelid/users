{
  "info": {
    "name": "Eventbrite Get Users User  Tracking Beacons",
    "_postman_id": "01f049e4-0b38-403c-8eac-233f7904ca74",
    "description": "Returns the list of tracking_beacon for the user :user_id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tracking",
      "item": [
        {
          "id": "b0cea7e0-5445-498c-89cd-29ad50b74e65",
          "name": "postTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/tracking_beacons/?event_id=%7B%7D&pixel_id=%7B%7D&tracking_type=%7B%7D&triggers=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Makes a new tracking beacon. Returns an tracking_beacon as tracking_beacon. Either event_id or user_id is required for each tracking beacon. If the event_id is provided, the tracking pixel will fire only for that event. If the user_id is provided, the tracking pixel will fire for all events organized by that user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bab7f91-202d-473e-a9c8-3bc2da91f586"
            }
          ]
        },
        {
          "id": "1a26f438-b904-4be9-a23d-5c43eef421d6",
          "name": "getTrackingBeaconsTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/tracking_beacons/:tracking_beacons_id/?return_fmt=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the tracking_beacon with the specified :tracking_beacons_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb9265d2-b568-433b-bfbc-89f5522f99ce"
            }
          ]
        },
        {
          "id": "cd844ce2-3a6a-4aae-94e3-b2f692664412",
          "name": "postTrackingBeaconsTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/tracking_beacons/:tracking_beacons_id/?event_id=%7B%7D&pixel_id=%7B%7D&tracking_type=%7B%7D&triggers=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the tracking_beacons with the specified :tracking_beacons_id. Though event_id and user_id are not individually required, it is a requirement to have a tracking beacon where either one must exist. Returns an tracking_beacon as tracking_beacon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b762157f-2150-41db-8ed1-37f68008dfea"
            }
          ]
        },
        {
          "id": "13e263f6-b82c-428e-8816-b6a5ec5b2b51",
          "name": "deleteTrackingBeaconsTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/tracking_beacons/:tracking_beacons_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the tracking_beacons with the specified :tracking_beacons_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0bd3d70-0be6-4537-8d73-accb567865a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "f88469eb-af4f-4e68-8780-28901d5db8cf",
          "name": "getEventsEventTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/events/:event_id/tracking_beacons/?return_fmt=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of tracking_beacon for the event :event_id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "823fa23a-4e7d-4741-bf7a-2867ceb89af9"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "ba65d0d5-7dab-4606-b93f-e249b5092a9a",
          "name": "getUsersUserTrackingBeacons",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/users/:user_id/tracking_beacons/?return_fmt=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of tracking_beacon for the user :user_id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9f44e19-4a02-4797-93db-d3d8f43f88da"
            }
          ]
        }
      ]
    }
  ]
}