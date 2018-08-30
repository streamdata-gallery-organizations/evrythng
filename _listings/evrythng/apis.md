---
name: EVRYTHNG
x-slug: evrythng
description: EVRYTHNG is the market leading internet of things platform for consumer
  product brands. Now individual product items can tell their stories to your business
  and your consumers throughout their lifecycle.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
x-kinRank: "7"
x-alexaRank: "686135"
tags: EVRYTHNG
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/apis.md
specificationVersion: "0.14"
apis:
- name: EVRYTHNG - /thngs (O)
  x-api-slug: thngs-get
  description: OPERATOR reads the list of all thngs in the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/thngs-get-openapi.md
- name: EVRYTHNG - /thngs (O)
  x-api-slug: thngs-post
  description: Creates a thng that is visible by no Applications
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/thngs-post-openapi.md
- name: EVRYTHNG - /products/{id} (O)
  x-api-slug: productsprod-id-get
  description: OPERATOR reads a specific product.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/productsprod-id-get-openapi.md
- name: EVRYTHNG - /auth/evrythng/users (A)
  x-api-slug: authevrythngusers-post
  description: APP creates a new EVRYTHNG user in it (using email/password).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/authevrythngusers-post-openapi.md
- name: EVRYTHNG - /users/{id} (O)
  x-api-slug: usersuser-id-get
  description: OPERATOR reads data a specific user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/usersuser-id-get-openapi.md
- name: EVRYTHNG - /user/{id}/validate (A)
  x-api-slug: authevrythngusersuser-idvalidate-post
  description: APP validates a user (which can then login & out).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/authevrythngusersuser-idvalidate-post-openapi.md
- name: EVRYTHNG - /products (A)
  x-api-slug: products-get
  description: APP Reads the list of all products visible.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/products-get-openapi.md
- name: EVRYTHNG - /products (O)
  x-api-slug: products-post
  description: OPERATOR creates a product visible in **NO** applications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/products-post-openapi.md
- name: EVRYTHNG - /actions/scans (U)
  x-api-slug: actionsscans-post
  description: |-
    **USER** creates a "scan" action on a thng.

    **ATTENTION -->** use a valid thng ID in the payload!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/actionsscans-post-openapi.md
- name: EVRYTHNG - /actions?project={id} (O)
  x-api-slug: actions-get
  description: '**OPERATOR** returns all the action types in the scope of an Application.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/actions-get-openapi.md
- name: EVRYTHNG - /actions?project={id} (O)
  x-api-slug: actions-post
  description: '**OPERATOR** creates a new custom action type for app ID (visible
    only by that app).'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/actions-post-openapi.md
- name: EVRYTHNG - /applications/ (O)
  x-api-slug: projectsproject-idapplications-post
  description: OPERATOR creates a new application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/projectsproject-idapplications-post-openapi.md
- name: EVRYTHNG - /projects/{id} (O)
  x-api-slug: projectsproject-id-get
  description: OPERATOR Reads a Specific Project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/projectsproject-id-get-openapi.md
- name: EVRYTHNG - /users/{id}/status (O)
  x-api-slug: usersuser-idstatus-get
  description: OPERATOR gets the status of a specific user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/usersuser-idstatus-get-openapi.md
- name: EVRYTHNG - /auth/evrythng (A)
  x-api-slug: authevrythng-post
  description: APP logs in an existing (and activated) user (with email/password).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/authevrythng-post-openapi.md
- name: EVRYTHNG - /projects/ (O)
  x-api-slug: projects-get
  description: OPERATOR reads the list of all Projects.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/projects-get-openapi.md
- name: EVRYTHNG - /projects/ (O)
  x-api-slug: projects-post
  description: OPERATOR creates a new project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/projects-post-openapi.md
- name: EVRYTHNG - /users (O)
  x-api-slug: users-get
  description: OPERATOR gets the list of all users of the engine.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/users-get-openapi.md
- name: EVRYTHNG - /applications/{id} (O)
  x-api-slug: projectsproject-idapplicationsapp-id-get
  description: OPERATOR reads a specific application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/projectsproject-idapplicationsapp-id-get-openapi.md
- name: EVRYTHNG - /thngs/{id}/location (U)
  x-api-slug: thngsthng-idlocation-put
  description: USER updates the location of a thng.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/thngsthng-idlocation-put-openapi.md
- name: EVRYTHNG - /auth/all/logout (U)
  x-api-slug: authalllogout-post
  description: USER logs himself out (which renders the user API Key invalid).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/evrythng/master/_listings/evrythng/authalllogout-post-openapi.md
x-common:
- type: x-deprecation
  url: https://developers.evrythng.com/docs/deprecation
- type: x-github
  url: https://github.com/evrythng
- type: x-postman-collection
  url: https://www.getpostman.com/collections/ba74e4cd196b0cffefec
- type: x-websub
  url: https://developers.evrythng.com/docs/pubsub
- type: x-api-gallery
  url: http://eventbrite.api.gallery.streamdata.io
- type: x-api-stack
  url: http://evrythng.stack.network
- type: x-authentication
  url: https://developers.evrythng.com/docs/authentication
- type: x-blog
  url: https://evrythng.com/blog/
- type: x-blog
  url: https://developers.evrythng.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/thngy
- type: x-email
  url: press@evrythng.com
- type: x-email
  url: privacy@evrythng.com
- type: x-security
  url: https://evrythng.com/securing-the-internet-of-things/
- type: x-support
  url: https://developers.evrythng.com/docs/support
- type: x-twitter
  url: https://twitter.com/EVRYTHNG
- type: x-website
  url: https://evrythng.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---