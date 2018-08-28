---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get project issue security levels
  description: |-
    Returns all [issue security](https://confluence.atlassian.com/x/J4lKLg) levels for the project that the currently authenticated user has access to. If the user does not have permission to see an issue security level, then that level is not returned. If the user lacks the _Set Issue Security_ permission, then an empty list is returned.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Set Issue Security_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
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
  /api/2/project/{projectKeyOrId}/issuesecuritylevelscheme:
    get:
      summary: Get project issue security scheme
      description: |-
        Returns the [issue security scheme](https://confluence.atlassian.com/x/J4lKLg) associated with the project.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or the _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectIssueSecurityLevelSchemeResource.getIssueSecurityScheme_get
      x-api-path-slug: api2projectprojectkeyoridissuesecuritylevelscheme-get
      parameters:
      - in: path
        name: projectKeyOrId
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
      - Issue
      - Security
      - Scheme
  /api/2/project/{projectKeyOrId}/securitylevel:
    get:
      summary: Get project issue security levels
      description: |-
        Returns all [issue security](https://confluence.atlassian.com/x/J4lKLg) levels for the project that the currently authenticated user has access to. If the user does not have permission to see an issue security level, then that level is not returned. If the user lacks the _Set Issue Security_ permission, then an empty list is returned.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Set Issue Security_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.securitylevel.ProjectSecurityLevelResource.getSecurityLevelsForProject_ge
      x-api-path-slug: api2projectprojectkeyoridsecuritylevel-get
      parameters:
      - in: path
        name: projectKeyOrId
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
      - Issue
      - Security
      - Levels
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