---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/favorite:
    get:
      summary: Get Favorite Contacts
      description: "Returns favorite contacts of the current extension. Favorite contacts
        include both company contacts (extensions) and personal contacts (address
        book records).\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadContacts] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [ReadPersonalContacts] permission for
        requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: listFavoriteContacts
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidfavorite-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Favorite
      - Contacts
    put:
      summary: Update Favorite Contacts
      description: "Updates favorite contacts of the current extension. Favorite contacts
        include both company contacts (extensions) and personal contacts (address
        book records).**Please note**: currently personal address book size is limited
        to 10 000 contacts.\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [records.extensionId] value is
        invalid\n\n\n400\nFAV-100\nContact not found\n\n\n400\nFAV-101\nMore than
        one contact with the same [records.extensionId]\n\n\n400\nFAV-102\n[records.extensionId]
        and [records.contactId] could not be specified for one contact simultaneously\n\n\n400\nFAV-103\nMore
        than one contact with the same [records.id]\n\n\n400\nFAV-104\nContact limit
        exceeded\n\n\n400\nFAV-105\nContact not found in federated directory\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [Contacts] permission\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: updateFavoriteContacts
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidfavorite-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Favorite
      - Contacts
---