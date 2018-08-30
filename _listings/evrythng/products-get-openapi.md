---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /products (A)
  description: APP Reads the list of all products visible.
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
  /thngs:
    get:
      summary: /thngs (O)
      description: OPERATOR reads the list of all thngs in the account.
      operationId: ThngsGet
      x-api-path-slug: thngs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Thngs
    post:
      summary: /thngs (O)
      description: Creates a thng that is visible by no Applications
      operationId: ThngsPost
      x-api-path-slug: thngs-post
      parameters:
      - in: header
        name: Accept
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
      - Thngs
  /products/{PROD_ID}:
    get:
      summary: /products/{id} (O)
      description: OPERATOR reads a specific product.
      operationId: ProductsByPRODIDGet
      x-api-path-slug: productsprod-id-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: PROD_ID
      responses:
        200:
          description: OK
      tags:
      - Products
      - PROD
      - ID
  /auth/evrythng/users:
    post:
      summary: /auth/evrythng/users (A)
      description: APP creates a new EVRYTHNG user in it (using email/password).
      operationId: AuthEvrythngUsersPost
      x-api-path-slug: authevrythngusers-post
      parameters:
      - in: header
        name: Accept
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
      - Auth
      - Evrythng
      - Users
  /users/{USER_ID}:
    get:
      summary: /users/{id} (O)
      description: OPERATOR reads data a specific user.
      operationId: UsersByUSERIDGet
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Users
      - USER
      - ID
  /auth/evrythng/users/{USER_ID}/validate:
    post:
      summary: /user/{id}/validate (A)
      description: APP validates a user (which can then login & out).
      operationId: AuthEvrythngUsersValidateByUSERIDPost
      x-api-path-slug: authevrythngusersuser-idvalidate-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Evrythng
      - Users
      - USER
      - ID
      - Validate
  /products:
    get:
      summary: /products (A)
      description: APP Reads the list of all products visible.
      operationId: ProductsGet2
      x-api-path-slug: products-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Products
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