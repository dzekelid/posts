{
  "info": {
    "name": "Pinboard Add New Bookmark",
    "_postman_id": "bf24bb77-ad5d-4e50-82b7-1de4742f4c0e",
    "description": "Add a new bookmark.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "5c04374f-922c-416c-9c5f-d77117e17078",
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
              "id": "41ad21a8-4504-4afd-8c76-0a2f43d5eabf"
            }
          ]
        },
        {
          "id": "f6775204-c386-4207-89b2-214e4e9eecc9",
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
              "id": "98af1c20-d70a-46b2-90ff-b6048a1489be"
            }
          ]
        }
      ]
    }
  ]
}