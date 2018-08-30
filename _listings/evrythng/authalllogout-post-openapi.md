---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /auth/all/logout (U)
  description: USER logs himself out (which renders the user API Key invalid).
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
    post:
      summary: /products (O)
      description: OPERATOR creates a product visible in **NO** applications.
      operationId: ProductsPost
      x-api-path-slug: products-post
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
      - Products
  /actions/scans:
    post:
      summary: /actions/scans (U)
      description: |-
        **USER** creates a "scan" action on a thng.

        **ATTENTION -->** use a valid thng ID in the payload!
      operationId: ActionsScansPost2
      x-api-path-slug: actionsscans-post
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
      - Actions
      - Scans
  /actions:
    get:
      summary: /actions?project={id} (O)
      description: '**OPERATOR** returns all the action types in the scope of an Application.'
      operationId: ActionsGet2
      x-api-path-slug: actions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: project
      responses:
        200:
          description: OK
      tags:
      - Actions
    post:
      summary: /actions?project={id} (O)
      description: '**OPERATOR** creates a new custom action type for app ID (visible
        only by that app).'
      operationId: ActionsPost2
      x-api-path-slug: actions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: project
      responses:
        200:
          description: OK
      tags:
      - Actions
  /projects/{PROJECT_ID}/applications/:
    post:
      summary: /applications/ (O)
      description: OPERATOR creates a new application.
      operationId: ProjectsApplicationsByPROJECTIDPost
      x-api-path-slug: projectsproject-idapplications-post
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
        name: PROJECT_ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Applications
  /projects/{PROJECT_ID}:
    get:
      summary: /projects/{id} (O)
      description: OPERATOR Reads a Specific Project.
      operationId: ProjectsByPROJECTIDGet
      x-api-path-slug: projectsproject-id-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: PROJECT_ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
  /users/{USER_ID}/status:
    get:
      summary: /users/{id}/status (O)
      description: OPERATOR gets the status of a specific user.
      operationId: UsersStatusByUSERIDGet
      x-api-path-slug: usersuser-idstatus-get
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
      - Status
  /auth/evrythng/:
    post:
      summary: /auth/evrythng (A)
      description: APP logs in an existing (and activated) user (with email/password).
      operationId: AuthEvrythngPost
      x-api-path-slug: authevrythng-post
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
  /projects/:
    get:
      summary: /projects/ (O)
      description: OPERATOR reads the list of all Projects.
      operationId: ProjectsGet
      x-api-path-slug: projects-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Projects
    post:
      summary: /projects/ (O)
      description: OPERATOR creates a new project.
      operationId: ProjectsPost
      x-api-path-slug: projects-post
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
      - Projects
  /users:
    get:
      summary: /users (O)
      description: OPERATOR gets the list of all users of the engine.
      operationId: UsersGet
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Users
  /projects/{PROJECT_ID}/applications/{APP_ID}:
    get:
      summary: /applications/{id} (O)
      description: OPERATOR reads a specific application.
      operationId: ProjectsApplicationsByPROJECTIDAndAPPIDGet
      x-api-path-slug: projectsproject-idapplicationsapp-id-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: APP_ID
      - in: header
        name: Content-Type
      - in: path
        name: PROJECT_ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Applications
      - APP
      - ID
  /thngs/{THNG_ID}/location:
    put:
      summary: /thngs/{id}/location (U)
      description: USER updates the location of a thng.
      operationId: ThngsLocationByTHNGIDPut
      x-api-path-slug: thngsthng-idlocation-put
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
        name: THNG_ID
      responses:
        200:
          description: OK
      tags:
      - Thngs
      - THNG
      - ID
      - Location
  /auth/all/logout:
    post:
      summary: /auth/all/logout (U)
      description: USER logs himself out (which renders the user API Key invalid).
      operationId: AuthAllLogoutPost
      x-api-path-slug: authalllogout-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Auth
      - ""
      - Logout
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