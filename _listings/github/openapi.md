---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers--over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories--with-the-collaborative-features-of-github-com-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code-
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/issues/{number}/labels:
    delete:
      summary: Delete Repos Owner Repo Issues Number Labels
      description: Remove all labels from an issue.
      operationId: remove-all-labels-from-an-issue
      x-api-path-slug: reposownerrepoissuesnumberlabels-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Labels
    get:
      summary: Get Repos Owner Repo Issues Number Labels
      description: List labels on an issue.
      operationId: list-labels-on-an-issue
      x-api-path-slug: reposownerrepoissuesnumberlabels-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Labels
    post:
      summary: Add Repos Owner Repo Issues Number Labels
      description: Add labels to an issue.
      operationId: add-labels-to-an-issue
      x-api-path-slug: reposownerrepoissuesnumberlabels-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Labels
    put:
      summary: Put Repos Owner Repo Issues Number Labels
      description: |-
        Replace all labels for an issue.
        Sending an empty array ([]) will remove all Labels from the Issue.
      operationId: replace-all-labels-for-an-issuesending-an-empty-array--will-remove-all-labels-from-the-issue
      x-api-path-slug: reposownerrepoissuesnumberlabels-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Labels
  /repos/{owner}/{repo}/issues/{number}/labels/{name}:
    delete:
      summary: Delete Repos Owner Repo Issues Number Labels Name
      description: Remove a label from an issue.
      operationId: remove-a-label-from-an-issue
      x-api-path-slug: reposownerrepoissuesnumberlabelsname-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: name
        description: Name of the label
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Labels
      - Name
  /repos/{owner}/{repo}/labels:
    get:
      summary: Get Repos Owner Repo Labels
      description: List all labels for this repository.
      operationId: list-all-labels-for-this-repository
      x-api-path-slug: reposownerrepolabels-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Labels
    post:
      summary: Add Repos Owner Repo Labels
      description: Create a label.
      operationId: create-a-label
      x-api-path-slug: reposownerrepolabels-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Labels
  /repos/{owner}/{repo}/labels/{name}:
    delete:
      summary: Delete Repos Owner Repo Labels Name
      description: Delete a label.
      operationId: delete-a-label
      x-api-path-slug: reposownerrepolabelsname-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: name
        description: Name of the label
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Labels
      - Name
    get:
      summary: Get Repos Owner Repo Labels Name
      description: Get a single label.
      operationId: get-a-single-label
      x-api-path-slug: reposownerrepolabelsname-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: name
        description: Name of the label
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Labels
      - Name
    patch:
      summary: Patch Repos Owner Repo Labels Name
      description: Update a label.
      operationId: update-a-label
      x-api-path-slug: reposownerrepolabelsname-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Name of the label
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Labels
      - Name
  /repos/{owner}/{repo}/milestones/{number}/labels:
    get:
      summary: Get Repos Owner Repo Milestones Number Labels
      description: Get labels for every issue in a milestone.
      operationId: get-labels-for-every-issue-in-a-milestone
      x-api-path-slug: reposownerrepomilestonesnumberlabels-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of milestone
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Milestones
      - Number
      - Labels
---