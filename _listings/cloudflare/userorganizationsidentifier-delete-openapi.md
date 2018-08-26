---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare Remove association to an organization
  version: 1.0.0
  description: Remove association to an organization
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/organizations:
    get:
      summary: List organizations the user is associated with
      description: List organizations the user is associated with
      operationId: cloudflare-userx27s-organizations-api
      x-api-path-slug: userorganizations-get
      parameters:
      - in: query
        name: direction
        description: Direction to order organizationsdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: name
        description: Organization NameCloudFlare, Inc
      - in: query
        name: order
        description: Field to order organizations bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of organizations per page20
      - in: query
        name: status
        description: Whether or not the user is a member of the organization or has
          an inivitation pendingmember
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Organizations
  /user/organizations/:identifier:
    delete:
      summary: Remove association to an organization
      description: Remove association to an organization
      operationId: cloudflare-userx27s-organizations-api
      x-api-path-slug: userorganizationsidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - User Organizations
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