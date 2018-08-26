---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/markets/ebay/fulfillment_policies/{id}:
    get:
      summary: Get fulfillment policy
      description: Get fulfillment policy for given ID.
      operationId: getRestMarketsEbayFulfillmentPolicies
      x-api-path-slug: restmarketsebayfulfillment-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Fulfillment
      - Policy
---