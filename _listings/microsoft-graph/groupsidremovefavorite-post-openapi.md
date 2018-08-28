---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Group Remove Favorite
  description: 'group: removeFavorite Remove the group from the list of the current
    user''s favorite groups. Supported for only Office 365 groups.'
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