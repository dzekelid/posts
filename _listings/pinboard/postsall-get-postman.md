{
  "info": {
    "name": "Pinboard Get All Posts",
    "_postman_id": "542a2399-5291-4169-af7f-496f83154358",
    "description": "Returns all bookmarks in the user's account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "22765768-2ebc-47fc-9bfd-523b354b394e",
          "name": "posts.update.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/update",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the most recent time a bookmark was added, updated or deleted. Use this before calling posts/all to see if the data has changed since the last fetch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a67cdb93-7177-4a9d-a911-48c2a7fec9dc"
            }
          ]
        },
        {
          "id": "e4b0109f-8afe-4bd0-a93c-f913352185a2",
          "name": "posts.add.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/add",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add a new bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe6a55ae-8f53-4408-a4c3-c587907ac3fc"
            }
          ]
        },
        {
          "id": "c44b20bd-56ec-4616-a11f-ea1358ab9d96",
          "name": "posts.delete.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/delete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "384d1d92-9f05-4ff1-8a6f-f8d7f9156b26"
            }
          ]
        },
        {
          "id": "c290fb95-d4ec-4d12-8b8c-d818bf0efa3e",
          "name": "posts.get.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/get",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one or more posts on a single day matching the arguments. If no date or url is given, date of most recent bookmark will be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c0220bf-889a-45db-8790-610304721947"
            }
          ]
        },
        {
          "id": "fd71c8b1-acd4-417a-adf9-72e8d0640691",
          "name": "posts.dates.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/dates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of dates with the number of posts at each date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33bdfe38-bc20-4b7d-bf1f-490aeb9716f0"
            }
          ]
        },
        {
          "id": "a19d0009-480f-4799-bc76-5ef1f33d6541",
          "name": "posts.recent.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/recent?count=count&tag=tag",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's most recent posts, filtered by tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "735efca5-ff09-4333-8266-f6fc6a7e474e"
            }
          ]
        },
        {
          "id": "54422b40-0f65-42e9-b09f-a4514bd3cad3",
          "name": "posts.all.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/all?fromdt=fromdt&meta=meta&results=results&start=start&tag=tag&todt=todt",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all bookmarks in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f840563d-f83d-482b-bbf7-9a262e318625"
            }
          ]
        }
      ]
    }
  ]
}