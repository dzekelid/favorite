---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/region/favourites:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetAllFavourites
      x-api-path-slug: apiregionfavourites-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
  /api/region/favourites/{favouriteRegionId}:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-get
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
---