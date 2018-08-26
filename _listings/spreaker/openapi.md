---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/lives/fan:
    get:
      summary: Get Favorite Live Episodes
      description: ""
      operationId: getUserUserLivesFan
      x-api-path-slug: useruser-idlivesfan-get
      parameters:
      - in: path
        name: /user/{user_id}/lives/fan
        description: Users id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Favorite
      - Live
      - Episodes
  /user/{user_id}/shows/fan:
    get:
      summary: Get Favorite Shows
      description: Retrieves the list of shows whose authors are followed by <user_id>.
      operationId: getUserUserShowsFan
      x-api-path-slug: useruser-idshowsfan-get
      parameters:
      - in: query
        name: latest_episode
        description: True (1) to enable the export of the latest episode
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Favorite
      - Shows
---