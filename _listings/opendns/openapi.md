---
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
---