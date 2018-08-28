swagger: "2.0"
x-collection-name: Gmail
x-complete: 1
info:
  title: Gmail
  version: 1.0.0
host: www.googleapis.com
basePath: /gmail/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/labels:
    get:
      summary: Get Labels
      description: Lists all labels in the user's mailbox.
      operationId: gmail.users.labels.list
      x-api-path-slug: useridlabels-get
      parameters:
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label
    post:
      summary: Create Label
      description: Creates a new label.
      operationId: gmail.users.labels.create
      x-api-path-slug: useridlabels-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label
  /{userId}/labels/{id}:
    delete:
      summary: Delete Lbel
      description: Immediately and permanently deletes the specified label and removes
        it from any messages and threads that it is applied to.
      operationId: gmail.users.labels.delete
      x-api-path-slug: useridlabelsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the label to delete
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label
    get:
      summary: Get Label
      description: Gets the specified label.
      operationId: gmail.users.labels.get
      x-api-path-slug: useridlabelsid-get
      parameters:
      - in: path
        name: id
        description: The ID of the label to retrieve
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label
    patch:
      summary: Update Label
      description: Updates the specified label. This method supports patch semantics.
      operationId: gmail.users.labels.patch
      x-api-path-slug: useridlabelsid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the label to update
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label
    put:
      summary: Update Label
      description: Updates the specified label.
      operationId: gmail.users.labels.update
      x-api-path-slug: useridlabelsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the label to update
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Label