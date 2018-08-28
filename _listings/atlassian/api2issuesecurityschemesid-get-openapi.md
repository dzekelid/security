---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get issue security scheme
  description: Returns the issue security scheme along with that are defined.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issuesecurityschemes:
    get:
      summary: Get issue security schemes
      description: Returns all issue security schemes that are defined.
      operationId: com.atlassian.jira.rest.v2.issue.IssueSecuritySchemeResource.getIssueSecuritySchemes_get
      x-api-path-slug: api2issuesecurityschemes-get
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Security
      - Schemes
  /api/2/issuesecurityschemes/{id}:
    get:
      summary: Get issue security scheme
      description: Returns the issue security scheme along with that are defined.
      operationId: com.atlassian.jira.rest.v2.issue.IssueSecuritySchemeResource.getIssueSecurityScheme_get
      x-api-path-slug: api2issuesecurityschemesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Security
      - Scheme
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