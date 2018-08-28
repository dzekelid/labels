---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Post Labels
  description: Post labels.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/labels:
    get:
      summary: Get Boards Labels
      description: Get boards labels.
      operationId: getBoardsLabelsByIdBoard
      x-api-path-slug: boardsidboardlabels-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: color, idBoard, name or uses'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
    post:
      summary: Post Boards Labels
      description: Post boards labels.
      operationId: addBoardsLabelsByIdBoard
      x-api-path-slug: boardsidboardlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Labels to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
  /boards/{idBoard}/labels/{idLabel}:
    get:
      summary: Get Boards Labels Label
      description: Get boards labels label.
      operationId: getBoardsLabelsByIdBoardByIdLabel
      x-api-path-slug: boardsidboardlabelsidlabel-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: color, idBoard, name or uses'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idLabel
        description: idLabel
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
      - Label
  /cards/{idCard}/idLabels:
    post:
      summary: Post Cards Labels
      description: Post cards labels.
      operationId: addCardsIdLabelsByIdCard
      x-api-path-slug: cardsidcardidlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Labels to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Labels
  /cards/{idCard}/idLabels/{idLabel}:
    delete:
      summary: Delete Cards Labels Label
      description: Delete cards labels label.
      operationId: deleteCardsIdLabelsByIdCardByIdLabel
      x-api-path-slug: cardsidcardidlabelsidlabel-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idLabel
        description: idLabel
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Labels
      - Label
  /cards/{idCard}/labels:
    post:
      summary: Post Cards Labels
      description: Post cards labels.
      operationId: addCardsLabelsByIdCard
      x-api-path-slug: cardsidcardlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Labels to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Labels
    put:
      summary: Put Cards Labels
      description: Put cards labels.
      operationId: updateCardsLabelsByIdCard
      x-api-path-slug: cardsidcardlabels-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Labels to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Labels
  /cards/{idCard}/labels/{color}:
    delete:
      summary: Delete Cards Labels Color
      description: Delete cards labels color.
      operationId: deleteCardsLabelsByIdCardByColor
      x-api-path-slug: cardsidcardlabelscolor-delete
      parameters:
      - in: path
        name: color
        description: color
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Labels
      - Color
  /labels:
    post:
      summary: Post Labels
      description: Post labels.
      operationId: addLabels
      x-api-path-slug: labels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Labels to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Labels
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