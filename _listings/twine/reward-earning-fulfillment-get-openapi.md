---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine List reward earning fulfillments
  description: Get a list of reward earning fulfillments matching the specified filters.
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reward_earning_fulfillment:
    post:
      summary: Create a reward earning fulfillment
      description: Create a reward earning fulfillment for a reward earning. There
        can only be one fulfillment for each earning.
      operationId: createRewardEarningFulfillment
      x-api-path-slug: reward-earning-fulfillment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Reward
      - Earning
      - Fulfillment
    get:
      summary: List reward earning fulfillments
      description: Get a list of reward earning fulfillments matching the specified
        filters.
      operationId: fetchRewardEarningFulfillments
      x-api-path-slug: reward-earning-fulfillment-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Reward
      - Earning
      - Fulfillments
  /reward_earning_fulfillment/{id}:
    get:
      summary: Get a reward earning fulfillment
      description: Get a reward earning fulfillment record by id.
      operationId: fetchRewardEarningFulfillment
      x-api-path-slug: reward-earning-fulfillmentid-get
      parameters:
      - in: path
        name: id
        description: Reward earning fulfillment identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Reward
      - Earning
      - Fulfillment
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