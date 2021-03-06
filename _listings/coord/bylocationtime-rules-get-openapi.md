---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Curb Search API Find the rules for curbs near a location at a certain
    time.
  description: |-
    Find the rules for a given curb at a given time and on a given day. You can also use this
    to find all of the places that it is possible to perform a given action (for instance, find
    all the loading zones, or everywhere with two-hour parking).
  version: 1.0.0
host: api.coord.co
basePath: /v1/search/curbs
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bybounds/time_rules:
    get:
      summary: Find the rules for all curbs within a bounding box at a particular
        time.
      description: Find the rules for all curbs within a bounding box at a particular
        time..
      operationId: get_at_time_by_bounds
      x-api-path-slug: byboundstime-rules-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Find
      - Rules
      - Curbs
      - Within
      - Bounding
      - Box
      - At
      - Particular
      - Time
  /bycurb/{id}/time_rules:
    get:
      summary: Find the rules on a single curb at a certain time.
      description: Find the rules on a single curb at a certain time..
      operationId: get_at_time_by_curb_id
      x-api-path-slug: bycurbidtime-rules-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Find
      - Rules
      - "On"
      - Single
      - Curb
      - At
      - Certain
      - Time
  /bylocation/time_rules:
    get:
      summary: Find the rules for curbs near a location at a certain time.
      description: |-
        Find the rules for a given curb at a given time and on a given day. You can also use this
        to find all of the places that it is possible to perform a given action (for instance, find
        all the loading zones, or everywhere with two-hour parking).
      operationId: get_at_time_by_location
      x-api-path-slug: bylocationtime-rules-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Find
      - Rulescurbs
      - Near
      - Location
      - At
      - Certain
      - Time
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