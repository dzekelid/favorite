swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{id}/addFavorite:
    post:
      summary: Group Add Favorite
      description: 'group: addFavorite Add the group to the list of the current user''s
        favorite groups. Supported for only Office 365 groups.'
      operationId: Group:AddFavorite
      x-api-path-slug: groupsidaddfavorite-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - ""
      - Favorite
  /groups/{id}/removeFavorite:
    post:
      summary: Group Remove Favorite
      description: 'group: removeFavorite Remove the group from the list of the current
        user''s favorite groups. Supported for only Office 365 groups.'
      operationId: Group:RemoveFavorite
      x-api-path-slug: groupsidremovefavorite-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Remove
      - Favorite