---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS IP Address History
  version: 1.0.0
  description: To help better understand how IP addresses are related to each other
    and to the regional registries, the API can provide data about ASN and IP relationships.
    You can also find out more about the IP space associated with an AS with this
    endpoint and correlate BGP routing information between AS.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bgp_routes/ip/{ip}/:
    get:
      summary: IP Address History
      description: To help better understand how IP addresses are related to each
        other and to the regional registries, the API can provide data about ASN and
        IP relationships. You can also find out more about the IP space associated
        with an AS with this endpoint and correlate BGP routing information between
        AS.
      operationId: ipAddressHistory
      x-api-path-slug: bgp-routesipip-get
      parameters:
      - in: path
        name: ip
        description: The IP Address
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
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