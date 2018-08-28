---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get all ledger postings in the suspense account
  version: 1.0.0
  description: Get all ledger postings in the suspense account.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/ledger:
    post:
      summary: Retrive ledger postings without account id
      description: Retrive ledger postings without account id.
      operationId: Account_GetAllLedgerBydataContract
      x-api-path-slug: apiaccountledger-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrive
      - Ledger
      - Postings
      - Without
      - Account
      - Id
  /api/posting/suspense:
    get:
      summary: Get all ledger postings in the suspense account
      description: Get all ledger postings in the suspense account.
      operationId: Posting_GetSuspensePostingsBypageSizeBypageNumber
      x-api-path-slug: apipostingsuspense-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ledger
      - Postings
      - In
      - Suspense
      - Account
  /api/posting/cash:
    get:
      summary: Get all postings in the cash account for the agent
      description: Get all postings in the cash account for the agent.
      operationId: Posting_GetCashFunds
      x-api-path-slug: apipostingcash-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Postings
      - In
      - Cash
      - Accountthe
      - Agent
  /api/account/{id}/ledger:
    post:
      summary: Retrieve ledger posting details for an account
      description: Retrieve ledger posting details for an account.
      operationId: Account_GetLedgerByidBydataContract
      x-api-path-slug: apiaccountidledger-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Ledger
      - Posting
      - Detailsan
      - Account
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