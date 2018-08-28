---
name: Context.IO
x-slug: context-io
description: Create simple email webhooks and code against a free, RESTful, IMAP API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
x-kinRank: "9"
x-alexaRank: "569975"
tags: Labels
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/apis.md
specificationVersion: "0.14"
apis:
- name: Context.IO - Get Accounts Sources Label
  x-api-slug: accountsidsourceslabel-get
  description: Gets parameters and status for an IMAP source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-get-openapi.md
- name: Context.IO - Put Accounts Sources Label
  x-api-slug: accountsidsourceslabel-put
  description: Modifies a data source on a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-put-openapi.md
- name: Context.IO - Delete Accounts Sources Label
  x-api-slug: accountsidsourceslabel-delete
  description: Removes a data source of an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-delete-openapi.md
- name: Context.IO - Get Accounts Sources Label Folders
  x-api-slug: accountsidsourceslabelfolders-get
  description: Lists folders in an IMAP source. Returns folders existing in a given
    IMAP account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfolders-get-openapi.md
- name: Context.IO - Put Accounts Sources Label Folders Folder
  x-api-slug: accountsidsourceslabelfoldersfolder-put
  description: |-
    Creates a folder on an IMAP source. A new folder can be added to an IMAP source by PUTting the desired path under the sources/folders resource.
    Working with server-specific hierarchy delimiters:
    IMAP servers are free to use the character they want as the folder hierarchy delimiter. The bad news is they don't use the same. The good news is you don't need to know this, we take care of it.

    Then what is that delim parameter for?
    Good question. By default, we expect you to specify the folder hierarchy using / as the hierarchy delimiter. For example, to create a folder called my folder under the folder base folder, you would call:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder/my+folder

    No matter what's the actual hierarchy delimiter the IMAP server expects, this call will work. However, say you need to use another character as the delimiter, here's how you'd do it:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder.my+folder?delim=.

    Both examples above are equivalent and will have the same result no matter what the IMAP server expects as the actual hierarchy delimiter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-openapi.md
- name: Context.IO - Get Accounts Sources Label Sync
  x-api-slug: accountsidsourceslabelsync-get
  description: Gets the sync status of a data source. Returns the timestamps for the
    last time the source has been synced with the origin mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-get-openapi.md
- name: Context.IO - Post Accounts Sources Label Sync
  x-api-slug: accountsidsourceslabelsync-post
  description: Triggers a sync of a data source. This will start a sync job for the
    source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-post-openapi.md
- name: Context.IO - Post Accounts Sources Label Sync
  x-api-slug: accountsidsourceslabelsync-post
  description: Triggers a sync of a data source. This will start a sync job for the
    source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-post-openapi.md
- name: Context.IO - Get Accounts Sources Label Sync
  x-api-slug: accountsidsourceslabelsync-get
  description: Gets the sync status of a data source. Returns the timestamps for the
    last time the source has been synced with the origin mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelsync-get-openapi.md
- name: Context.IO - Put Accounts Sources Label Folders Folder
  x-api-slug: accountsidsourceslabelfoldersfolder-put
  description: |-
    Creates a folder on an IMAP source. A new folder can be added to an IMAP source by PUTting the desired path under the sources/folders resource.
    Working with server-specific hierarchy delimiters:
    IMAP servers are free to use the character they want as the folder hierarchy delimiter. The bad news is they don't use the same. The good news is you don't need to know this, we take care of it.

    Then what is that delim parameter for?
    Good question. By default, we expect you to specify the folder hierarchy using / as the hierarchy delimiter. For example, to create a folder called my folder under the folder base folder, you would call:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder/my+folder

    No matter what's the actual hierarchy delimiter the IMAP server expects, this call will work. However, say you need to use another character as the delimiter, here's how you'd do it:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder.my+folder?delim=.

    Both examples above are equivalent and will have the same result no matter what the IMAP server expects as the actual hierarchy delimiter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-openapi.md
- name: Context.IO - Get Accounts Sources Label Folders
  x-api-slug: accountsidsourceslabelfolders-get
  description: Lists folders in an IMAP source. Returns folders existing in a given
    IMAP account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabelfolders-get-openapi.md
- name: Context.IO - Delete Accounts Sources Label
  x-api-slug: accountsidsourceslabel-delete
  description: Removes a data source of an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-delete-openapi.md
- name: Context.IO - Put Accounts Sources Label
  x-api-slug: accountsidsourceslabel-put
  description: Modifies a data source on a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-put-openapi.md
- name: Context.IO - Get Accounts Sources Label
  x-api-slug: accountsidsourceslabel-get
  description: Gets parameters and status for an IMAP source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/context-io/accountsidsourceslabel-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://constant.contact.api.gallery.streamdata.io
- type: x-api-stack
  url: http://context.io.stack.network
- type: x-base
  url: https://api.context.io/
- type: x-blog
  url: http://blog.context.io/
- type: x-blog-rss
  url: http://blog.context.io/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/product/context-io
- type: x-crunchbase
  url: https://crunchbase.com/organization/context-io
- type: x-documentation
  url: http://context.io/docs/2.0
- type: x-email
  url: hello@context.io
- type: x-email
  url: support@context.io
- type: x-email
  url: business@context.io
- type: x-faq
  url: http://context.io/privacy-faq
- type: x-github
  url: https://github.com/contextio
- type: x-ios-library
  url: https://github.com/contextio/contextio-ios
- type: x-node-js-library
  url: https://github.com/contextio/ContextIO-node
- type: x-php-library
  url: https://github.com/contextio/PHP-ContextIO
- type: x-pricing
  url: http://context.io/pricing
- type: x-privacy
  url: http://www.returnpath.com/privacy-policy-data
- type: x-python-library
  url: https://github.com/contextio/Python-ContextIO
- type: x-ruby-library
  url: https://github.com/contextio/contextio-ruby
- type: x-selfservice-registration
  url: http://context.io/#signup
- type: x-terms-of-service
  url: http://context.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/contextio
- type: x-website
  url: http://context.io/
- type: x-website
  url: http://context.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---