{
  "info": {
    "name": "Pinboard Get Posts",
    "_postman_id": "b246f149-ac5d-4ee7-b262-6457ddcbe78a",
    "description": "Returns one or more posts on a single day matching the arguments. If no date or url is given, date of most recent bookmark will be used.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "f24b6562-cfeb-4ee4-9594-dfdc9cfe964d",
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
              "id": "8c545b3a-e352-45ed-87b4-3a14747da227"
            }
          ]
        },
        {
          "id": "b89b5492-e867-4966-a2d3-85c51d44330a",
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
              "id": "66fed494-6257-4553-b1cb-89682445e959"
            }
          ]
        },
        {
          "id": "b70b0617-f656-41f3-9c25-c13a1808ff35",
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
              "id": "fc721f67-3cf8-4ce6-ac4e-fc124a2a35d0"
            }
          ]
        },
        {
          "id": "4799880a-3ae6-44cb-b0b1-95d71002e88c",
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
              "id": "cdc0a750-1bfb-470f-a536-eabaf26421ae"
            }
          ]
        }
      ]
    }
  ]
}