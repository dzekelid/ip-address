---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
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
    post:
      summary: Add SIP IP Access Control List IP Address
      description: Change the description or IP address of a given IpAddress instance
        resource
      operationId: change-the-description-or-ip-address-of-a-given-ipaddress-instance-resource
      x-api-path-slug: accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-post
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
---