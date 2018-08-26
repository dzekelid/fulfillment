---
swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
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
---