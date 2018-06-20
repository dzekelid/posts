{
  "info": {
    "name": "Pinboard Get Recent Posts",
    "_postman_id": "63b406a0-f748-45ef-8753-2debc00eb8c9",
    "description": "Returns a list of the user's most recent posts, filtered by tag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "425f64d0-7971-4fa4-a243-5430fe3db93f",
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
              "id": "e79aa469-12c8-4124-9439-15ba313721e6"
            }
          ]
        },
        {
          "id": "6bd0d040-026d-404f-9e43-3a4e95bd45b5",
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
              "id": "42b18834-76e7-4594-ad22-ab3e4d7029b5"
            }
          ]
        },
        {
          "id": "430e1c01-019a-4b91-939f-44b7bfc04653",
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
              "id": "29a37606-7bca-4146-8e42-8a43e60cd736"
            }
          ]
        },
        {
          "id": "5f046537-ed5a-4645-b024-6cb059dc01b3",
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
              "id": "406f6c86-94b3-48d6-a05b-69b1940a18a5"
            }
          ]
        },
        {
          "id": "03fa82f0-77a7-430a-9fe4-fa9199a4f5fa",
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
              "id": "425959a9-c757-4fc6-8bff-1f532c25168b"
            }
          ]
        },
        {
          "id": "2c3e06a3-7b97-48c1-91f9-1404a476dc2e",
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
              "id": "bc47b259-2e1b-4923-9c41-c38257c65325"
            }
          ]
        }
      ]
    }
  ]
}