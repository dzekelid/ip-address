---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Delete SIP IP Access Control List IP Address
  description: Deletes an IP address entry from the list.
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/IpAccessControlLists:
    post:
      summary: Add SIP IP Access Control List
      description: Create a new IpAccessControlList resource.nnWhen created, the list
        will contain no IP addresses. You will need to add IP addresses to the list
        for it to be active. To add IP addresses, you will need to POST to the IpAddresses
        List subresource.n
      operationId: create-a-new-ipaccesscontrollist-resourcewhen-created-the-list-will-contain-no-ip-addresses-you-will
      x-api-path-slug: accountsaccountsidsipipaccesscontrollists-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - SIP IP Access Control Lists
  /Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses/{IpAddressSid}:
    delete:
      summary: Delete SIP IP Access Control List IP Address
      description: Deletes an IP address entry from the list.
      operationId: deletes-an-ip-address-entry-from-the-list
      x-api-path-slug: accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: IpAccessControlListSid
        description: A 34 character string that uniquely identifies the SIP IP access
          control list
      - in: path
        name: IpAddressSid
        description: A 34 character string that uniquely identifies the SIP IP access
          control list
      responses:
        200:
          description: OK
      tags:
      - SIP IP Access Control Lists
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