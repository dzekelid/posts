{
  "info": {
    "name": "Pinboard Update Tag",
    "_postman_id": "0e0413fc-3c91-41db-b746-2af2fa3687d3",
    "description": "Returns the most recent time a bookmark was added, updated or deleted. Use this before calling posts/all to see if the data has changed since the last fetch.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "c0925356-3eb3-448e-85cd-f658a2fac8e9",
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
              "id": "d18099ce-6a51-4639-af8f-93aefb68bb47"
            }
          ]
        }
      ]
    }
  ]
}