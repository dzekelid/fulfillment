---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Update tracking number for a fulfillment.
  description: Update tracking number for a fulfillment..
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
  /admin/orders/4528049998/fulfillments/3770145678/complete.json:
    post:
      summary: Complete a fulfillment.
      description: Complete a fulfillment..
      operationId: postAdminOrders4528049998Fulfillments3770145678Complete.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678complete-json-post
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
      - Complete
      - Fulfillment
  /admin/orders/4495703502/fulfillments/3763917198/events/9519874062.json:
    delete:
      summary: Delete a fulfillment event.
      description: Delete a fulfillment event..
      operationId: deleteAdminOrders4495703502Fulfillments3763917198Events9519874062.json
      x-api-path-slug: adminorders4495703502fulfillments3763917198events9519874062-json-delete
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
      - Event
  /admin/fulfillment_services/1357646.json:
    get:
      summary: Get a single fulfillment service by its ID
      description: Get a single fulfillment service by its id.
      operationId: getAdminFulfillmentServices1357646.json
      x-api-path-slug: adminfulfillment-services1357646-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Fulfillment
      - Service
      - By
      - Its
      - ID
    put:
      summary: Update a fulfillment service
      description: Update a fulfillment service.
      operationId: putAdminFulfillmentServices1357646.json
      x-api-path-slug: adminfulfillment-services1357646-json-put
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
    delete:
      summary: Destroy a fulfillment service
      description: Destroy a fulfillment service.
      operationId: deleteAdminFulfillmentServices1357646.json
      x-api-path-slug: adminfulfillment-services1357646-json-delete
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
      - Destroy
      - Fulfillment
      - Service
  /admin/orders/4528049998/fulfillments/3770145678.json:
    get:
      summary: Get the Representation of a specific fulfillment.
      description: Get the representation of a specific fulfillment..
      operationId: getAdminOrders4528049998Fulfillments3770145678.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Representation
      - Specific
      - Fulfillment
    put:
      summary: Update tracking number for a fulfillment.
      description: Update tracking number for a fulfillment..
      operationId: putAdminOrders4528049998Fulfillments3770145678.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678-json-put
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
      - Tracking
      - Numbera
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