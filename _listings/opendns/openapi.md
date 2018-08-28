swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 1
info:
  title: OpenDNS
  version: 1.0.0
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