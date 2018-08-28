swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/labels:
    get:
      summary: Get Projects Labels
      description: Get all labels of the project
      operationId: getV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    post:
      summary: Post Projects Labels
      description: Post projects labels.
      operationId: postV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-post
      parameters:
      - in: formData
        name: color
        description: 'The color of the label given in 6-digit hex notation with leading
          # sign (e'
      - in: formData
        name: description
        description: The description of label to be created
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: The name of the label to be created
      - in: formData
        name: priority
        description: The priority of the label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    delete:
      summary: Delete Projects Labels
      description: Delete an existing label
      operationId: deleteV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: name
        description: The name of the label to be deleted
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    put:
      summary: Put Projects Labels
      description: Update an existing label. At least one optional parameter is required.
      operationId: putV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-put
      parameters:
      - in: formData
        name: color
        description: 'The new color of the label given in 6-digit hex notation with
          leading # sign (e'
      - in: formData
        name: description
        description: The new description of label
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: The name of the label to be updated
      - in: formData
        name: new_name
        description: The new name of the label
      - in: formData
        name: priority
        description: The priority of the label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
  /v3/projects/{id}/labels/{subscribable_id}/subscription:
    post:
      summary: Post Projects Labels Subscribable Subscription
      description: Post projects labels subscribable subscription.
      operationId: postV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Labels Subscribable Subscription
      description: Delete projects labels subscribable subscription.
      operationId: deleteV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription