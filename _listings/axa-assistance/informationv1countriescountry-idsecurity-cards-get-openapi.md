---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Retrieve security information for a country
  description: Retrieve security information for a country
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /information/v1/countries/{country_id}/security_cards:
    get:
      summary: Retrieve security information for a country
      description: Retrieve security information for a country
      operationId: getInformationV1CountriesCountry_idSecurity_cards
      x-api-path-slug: informationv1countriescountry-idsecurity-cards-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      - in: path
        name: country_id
        description: country id
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - security
      - informationa
      - country
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