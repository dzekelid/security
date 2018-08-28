---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS Security Information
  version: 1.0.0
  description: The security information API method contains multiple scores or security
    features, each of which can be used to determine relevant datapoints to build
    insight on the reputation or security risk posed by the site. No one security
    information feature is conclusive, instead these features should be looked at
    in conjunction with one another as part of your security research.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /security/{name}/:
    get:
      summary: Security Information
      description: The security information API method contains multiple scores or
        security features, each of which can be used to determine relevant datapoints
        to build insight on the reputation or security risk posed by the site. No
        one security information feature is conclusive, instead these features should
        be looked at in conjunction with one another as part of your security research.
      operationId: securityInformation
      x-api-path-slug: securityname-get
      parameters:
      - in: path
        name: Domain Name
        description: Domain Name
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Security
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