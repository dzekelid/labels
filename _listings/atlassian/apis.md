---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Labels
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Add labels to content
  x-api-slug: contentidlabel-post
  description: "Adds labels to a piece of content. Does not modify the existing labels.\n\nNotes:\n\n-
    Labels can also be added when creating content ([Create content](#api-content-post)).\n-
    Labels can be updated when updating content ([Update content](#api-content-id-put)).
    \nThis will delete the existing labels and replace them with the labels in \nthe
    request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-post-openapi.md
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Get label watch status
  x-api-slug: userwatchlabellabelname-get
  description: "Returns whether a user is watching a label. Choose the user by doing
    one \nof the following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-openapi.md
- name: The Confluence Cloud REST API - Add label watcher
  x-api-slug: userwatchlabellabelname-post
  description: "Adds a user as a watcher to a label. Choose the user by doing one
    of the \nfollowing:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\nNote, you must add the `X-Atlassian-Token: no-check` header
    when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-openapi.md
- name: The Confluence Cloud REST API - Remove label watcher
  x-api-slug: userwatchlabellabelname-delete
  description: "Removes a user as a watcher from a label. Choose the user by doing
    one of \nthe following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label watcher
  x-api-slug: userwatchlabellabelname-delete
  description: "Removes a user as a watcher from a label. Choose the user by doing
    one of \nthe following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label watcher
  x-api-slug: userwatchlabellabelname-delete
  description: "Removes a user as a watcher from a label. Choose the user by doing
    one of \nthe following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-delete-openapi.md
- name: The Confluence Cloud REST API - Add label watcher
  x-api-slug: userwatchlabellabelname-post
  description: "Adds a user as a watcher to a label. Choose the user by doing one
    of the \nfollowing:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\nNote, you must add the `X-Atlassian-Token: no-check` header
    when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-openapi.md
- name: The Confluence Cloud REST API - Add label watcher
  x-api-slug: userwatchlabellabelname-post
  description: "Adds a user as a watcher to a label. Choose the user by doing one
    of the \nfollowing:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\nNote, you must add the `X-Atlassian-Token: no-check` header
    when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-post-openapi.md
- name: The Confluence Cloud REST API - Get label watch status
  x-api-slug: userwatchlabellabelname-get
  description: "Returns whether a user is watching a label. Choose the user by doing
    one \nof the following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-openapi.md
- name: The Confluence Cloud REST API - Get label watch status
  x-api-slug: userwatchlabellabelname-get
  description: "Returns whether a user is watching a label. Choose the user by doing
    one \nof the following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/userwatchlabellabelname-get-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/atlassian/contentidlabel-delete-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---