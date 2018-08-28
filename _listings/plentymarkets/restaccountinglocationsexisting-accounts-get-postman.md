{
  "info": {
    "name": "Plentymarkets Get all unique posting accounts",
    "_postman_id": "078643e9-5c5e-4575-b663-9e5bb6a41d9d",
    "description": "Get all unique posting accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "bf5c6464-8fea-446c-a74d-4f1318a618fc",
          "name": "getRestAccountingLocationsExistingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/existing_accounts",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all unique posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02f4db87-b481-4e39-ab1d-6192db971556"
            }
          ]
        }
      ]
    }
  ]
}