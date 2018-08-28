{
  "info": {
    "name": "Product Hunt Posts",
    "_postman_id": "f16f2c4e-892a-4260-bb3d-ce9835d0e2a4",
    "description": "Get posts by category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "ed6b734f-4874-410e-a353-2804658b818d",
          "name": "users.username.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.producthunt.com",
              "path": [
                "v1",
                "users/:username"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e3326d5-ea41-4fe2-90e2-c0e521b8c86c"
            }
          ]
        }
      ]
    },
    {
      "name": "Posts",
      "item": [
        {
          "id": "bf5d36aa-7535-4fcf-a2aa-e94540793d51",
          "name": "categories.category.posts.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.producthunt.com",
              "path": [
                "v1",
                "categories/:category/posts"
              ],
              "query": [
                {
                  "key": "days_ago",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get posts by category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "030567fd-1dbf-448e-8b44-6b9658960d50"
            }
          ]
        }
      ]
    }
  ]
}