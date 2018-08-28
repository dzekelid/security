---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Gets Email Sync Security Credentials
  version: 1.0.0
  description: Gets email sync security credentials.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/updateportalcustomisation:
    put:
      summary: "THIS IS A TEMPORARY ENDPOINT TO Update a portal customisation against
        a brand within a branch.\r\nPLEASE NOTE: This will be replaced by a FE Tool
        in future. If not, Security must be improved."
      description: "This is a temporary endpoint to update a portal customisation
        against a brand within a branch.\r\nplease note: this will be replaced by
        a fe tool in future. if not, security must be improved.."
      operationId: Agency_UpdatePortalCustomisationByportalCustomisation
      x-api-path-slug: apiagencyupdateportalcustomisation-put
      parameters:
      - in: body
        name: portalCustomisation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - THIS
      - IS
      - TEMPORARY
      - ENDPOINT
      - TO
      - ""
      - Portal
      - Customisation
      - Against
      - Brand
      - Within
      - Branch
      - PLEASE
      - 'NOTE:'
      - This
      - Will
      - Be
      - Replaced
      - By
      - FE
      - Tool
      - In
      - Future
      - ""
      - If
      - Not
      - ""
      - Security
      - Must
      - Be
      - Improved
  /api/credentials/upsertusernamepassword:
    post:
      summary: Creates or Updates Security Credentials
      description: Creates or updates security credentials.
      operationId: Credentials_UpsertUsernamePasswordBycredentialDataContract
      x-api-path-slug: apicredentialsupsertusernamepassword-post
      parameters:
      - in: body
        name: credentialDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Security
      - Credentials
  /api/credentials/emailsync/usernamepassword:
    get:
      summary: Gets Email Sync Security Credentials
      description: Gets email sync security credentials.
      operationId: Credentials_EmailSyncUsernamePasswordBycredentialDataContract.usernameBycredentialDataContract.passw
      x-api-path-slug: apicredentialsemailsyncusernamepassword-get
      parameters:
      - in: query
        name: credentialDataContract.password
      - in: query
        name: credentialDataContract.username
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Email
      - Sync
      - Security
      - Credentials
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