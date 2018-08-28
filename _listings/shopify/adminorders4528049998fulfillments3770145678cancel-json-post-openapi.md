---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Cancel a fulfillment.
  description: Cancel a fulfillment..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/fulfillment_services.json:
    get:
      summary: List your app's fulfillment services
      description: List your app's fulfillment services.
      operationId: getAdminFulfillmentServices.json
      x-api-path-slug: adminfulfillment-services-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Your
      - Apps
      - Fulfillment
      - Services
    post:
      summary: Create a fulfillment service
      description: Create a fulfillment service.
      operationId: postAdminFulfillmentServices.json
      x-api-path-slug: adminfulfillment-services-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Fulfillment
      - Service
  /admin/orders/4528049998/fulfillments/3770145678/cancel.json:
    post:
      summary: Cancel a fulfillment.
      description: Cancel a fulfillment..
      operationId: postAdminOrders4528049998Fulfillments3770145678Cancel.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678cancel-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Cancel
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