---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Sources Label Folders
  description: Lists folders in an IMAP source. Returns folders existing in a given
    IMAP account.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/sources/{label}:
    get:
      summary: Get Accounts Sources Label
      description: Gets parameters and status for an IMAP source.
      operationId: getAccountSource_
      x-api-path-slug: accountsidsourceslabel-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
    put:
      summary: Put Accounts Sources Label
      description: Modifies a data source on a given account.
      operationId: modifyAccountSource_
      x-api-path-slug: accountsidsourceslabel-put
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      - in: query
        name: password
        description: New password for this source
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key used to obtain the the token and token
          secret above for that account
      - in: query
        name: provider_token
        description: An OAuth token obtained from the IMAP account provider to be
          used to authentify on this email account
      - in: query
        name: provider_token_secret
        description: An OAuth token secret obtained from the IMAP account provider
          to be used to authentify on this email account
      - in: query
        name: service_level
        description: Changes the service level for the source
      - in: query
        name: status
        description: If the status of the source is TEMP_DISABLED or DISABLED
      - in: query
        name: sync_period
        description: Changes the period at which the Context
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
    delete:
      summary: Delete Accounts Sources Label
      description: Removes a data source of an account.
      operationId: removeAccountSource_
      x-api-path-slug: accountsidsourceslabel-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
  /accounts/{id}/sources/{label}/folders:
    get:
      summary: Get Accounts Sources Label Folders
      description: Lists folders in an IMAP source. Returns folders existing in a
        given IMAP account.
      operationId: listAccountSourceFolders_
      x-api-path-slug: accountsidsourceslabelfolders-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Folders
  /accounts/{id}/sources/{label}/folders/{folder}:
    put:
      summary: Put Accounts Sources Label Folders Folder
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
      operationId: createAccountSourceFolder_
      x-api-path-slug: accountsidsourceslabelfoldersfolder-put
      parameters:
      - in: query
        name: delim
        description: If / isnt fancy enough as a hierarchy delimiter when specifying
          the folder you want to create, youre free to use what you want, just make
          sure you set this delim parameter to tell us what youre using
      - in: path
        name: folder
        description: The full folder path you want to create
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Folders
      - Folder
  /accounts/{id}/sources/{label}/sync:
    get:
      summary: Get Accounts Sources Label Sync
      description: Gets the sync status of a data source. Returns the timestamps for
        the last time the source has been synced with the origin mailbox.
      operationId: getAccountSourceSyncStatus_
      x-api-path-slug: accountsidsourceslabelsync-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
    post:
      summary: Post Accounts Sources Label Sync
      description: Triggers a sync of a data source. This will start a sync job for
        the source.
      operationId: Create_syncAccountSource_
      x-api-path-slug: accountsidsourceslabelsync-post
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
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