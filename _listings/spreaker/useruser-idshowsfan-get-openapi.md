---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Get Favorite Shows
  version: v1
  description: Retrieves the list of shows whose authors are followed by <user_id>.
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