{
  "info": {
    "name": "Twilio Update Queue Members In Front",
    "_postman_id": "04d07587-cbb2-414c-af16-59b7eede22aa",
    "description": "Posting a URL and Method to a Queue instance will dequeue a member from anqueue and have the members call begin executing the TwiML document at that URLnWhen dequeuing the Front of the queue, the next call in the queue will be redirected.n",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "queues",
      "item": [
        {
          "id": "d04185db-7456-4b0a-8beb-0cb79f661ac4",
          "name": "posting-a-url-and-method-to-a-queue-instance-will-dequeue-a-member-from-aqueue-and-have-the-members-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Queues/:QueueSid/Members/Front"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "QueueSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posting a URL and Method to a Queue instance will dequeue a member from anqueue and have the members call begin executing the TwiML document at that URLnWhen dequeuing the Front of the queue, the next call in the queue will be redirected"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"members\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 201,
              "name": "Response_201",
              "id": "9486797c-cbbb-4ed1-abdc-b16c40090b1a"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The data given in the POST or PUT failed validation",
              "code": 400,
              "name": "Response_400",
              "id": "f0858d28-3691-4f1b-8c1b-e794d19131b8"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The supplied credentials, if any, are not sufficient to create or update the resource",
              "code": 401,
              "name": "Response_401",
              "id": "1c0ebeb1-88a3-4068-b1fc-641f75c309d4"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You know this one",
              "code": 404,
              "name": "Response_404",
              "id": "4cd431aa-6351-4ff7-9d1b-079f50746c04"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You can't POST or PUT to the resource",
              "code": 405,
              "name": "Response_405",
              "id": "f6ed8de4-ad98-4dcd-a828-a8189ba44c42"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "Your application is sending too many simultaneous requests",
              "code": 429,
              "name": "Response_429",
              "id": "823b349a-adce-4a09-b780-7bb299ba5e2f"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We couldn't create or update the resource",
              "code": 500,
              "name": "Response_500",
              "id": "37bf1efe-74a0-43f1-ba0c-cd4cfc3e0c23"
            }
          ]
        }
      ]
    }
  ]
}