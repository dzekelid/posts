---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get all posting accounts by locationId
  description: Get all posting accounts by locationid.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/locations/existing_accounts:
    get:
      summary: Get all unique posting accounts
      description: Get all unique posting accounts.
      operationId: getRestAccountingLocationsExistingAccounts
      x-api-path-slug: restaccountinglocationsexisting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Unique
      - Posting
      - Accounts
  /rest/accounting/locations/posting_accounts:
    get:
      summary: Get all posting accounts
      description: Get all posting accounts.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
    post:
      summary: Save posting accounts
      description: Save posting accounts.
      operationId: postRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Posting
      - Accounts
  /rest/accounting/locations/posting_accounts/{id}:
    delete:
      summary: Delete an posting account
      description: Delete an posting account.
      operationId: deleteRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Account
    get:
      summary: Gets posting account by the unique id
      description: Gets posting account by the unique id.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Posting
      - Account
      - By
      - Unique
      - Id
  /rest/accounting/locations/{locationId}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId
      description: Get all posting accounts by locationid.
      operationId: getRestAccountingLocationsLocationAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidposting-accounts-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
  /rest/accounting/locations/{locationId}/posting_key_configurations:
    get:
      summary: Get a posting key configuration of an accounting location
      description: Gets a posting key configuration of an accounting location. The
        ID of the accounting location has to be specified. The posting key configuration
        can contain up to 4 posting keys.
      operationId: getRestAccountingLocationsLocationAddingKeyConfigurations
      x-api-path-slug: restaccountinglocationslocationidposting-key-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Key
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/{type}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId and type
      description: Get all posting accounts by locationid and type.
      operationId: getRestAccountingLocationsLocationTypeAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidtypeposting-accounts-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
      - Type
  /rest/accounting/locations/{webstoreId}/{countryId}/posting_accounts:
    get:
      summary: Get all posting accounts for a country of a webstore
      description: Get all posting accounts for a country of a webstore.
      operationId: getRestAccountingLocationsWebstoreCountryAddingAccounts
      x-api-path-slug: restaccountinglocationswebstoreidcountryidposting-accounts-get
      parameters:
      - in: query
        name: $webstoreId
        description: The ID of the webstore
      - in: path
        name: countryId
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accountsa
      - Country
      - Of
      - Webstore
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---