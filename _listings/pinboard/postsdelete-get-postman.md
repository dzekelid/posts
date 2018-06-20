{
  "info": {
    "name": "Pinboard Delete a Post",
    "_postman_id": "72e35a6a-250b-4263-b37a-94e3b14899ce",
    "description": "Delete a bookmark.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "1baec685-3d8a-48eb-8c2f-0698afc75bb5",
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
              "id": "b90253fb-c309-4d8b-b332-0b3574961d72"
            }
          ]
        },
        {
          "id": "4537da91-3e86-4ab8-a2b7-4817ac92cece",
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
              "id": "31b7b8df-a19a-4dd4-b9e8-ee1639e7b5af"
            }
          ]
        },
        {
          "id": "2580daaa-2146-443f-9c42-be5519c6d35f",
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
              "id": "2793991c-c190-45ea-a277-1c59db6dbe2e"
            }
          ]
        }
      ]
    }
  ]
}