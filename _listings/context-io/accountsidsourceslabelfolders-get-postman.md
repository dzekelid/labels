{
  "info": {
    "name": "Context.IO Get Accounts Sources Label Folders",
    "_postman_id": "ef87f50c-9c0f-428b-950a-55bba07db57e",
    "description": "Lists folders in an IMAP source. Returns folders existing in a given IMAP account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "de672b96-589e-4775-9187-106e97c14db0",
          "name": "listAccounts_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&limit=%7B%7D&offset=%7B%7D&status=%7B%7D&status_ok=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c75578d-5e04-4140-a9f6-145b5cf9039e"
            }
          ]
        },
        {
          "id": "47c36997-30d6-4dc1-ab64-9ac23360611d",
          "name": "addAccount_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&token=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5acc1479-9516-4298-b503-6932bc8b4982"
            }
          ]
        },
        {
          "id": "b56c5d8c-abc6-420e-a70d-21674abc0765",
          "name": "getAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details about a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2835ed9-1138-4945-99ab-0b7ba565698a"
            }
          ]
        },
        {
          "id": "9a9886e3-9051-4873-8e55-fb1c429ac49e",
          "name": "modifyAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "query": [
                {
                  "key": "first_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "last_name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d50659bc-776b-4f25-899c-bda08c1980d5"
            }
          ]
        },
        {
          "id": "1a6c1913-e424-4e75-882c-f3a08a889bb0",
          "name": "removeAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "518d2438-3de5-4d63-a94e-5c99879c0d77"
            }
          ]
        },
        {
          "id": "25d6724d-bd8f-4e02-bfbe-b596acf591f5",
          "name": "listAccountConnectTokens_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists connect tokens created for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f1057cd-1072-47aa-9061-f906742abad6"
            }
          ]
        },
        {
          "id": "5e95d99d-be75-4303-a59c-09e91de32c65",
          "name": "Create_obtainNewAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens"
              ],
              "query": [
                {
                  "key": "callback_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "last_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_level",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains a new connect_token for a specific account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e780ec45-5997-4e49-a1d4-d01be81e369a"
            }
          ]
        },
        {
          "id": "32a9008b-df6f-4878-aec8-477fd2a2c523",
          "name": "getAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens/:token"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given connect token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f8297ca-38ba-4e4e-adf1-1497f69f00ed"
            }
          ]
        },
        {
          "id": "55dfd5c4-4a87-41f2-9ace-02ae0b34842a",
          "name": "removeAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens/:token"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a given connect token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71a19c47-4ed9-40ee-99bf-45bf8a144939"
            }
          ]
        },
        {
          "id": "5d4fa1da-73ae-4a85-a992-0527c69b4957",
          "name": "listAccountContacts_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts"
              ],
              "query": [
                {
                  "key": "active_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "active_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists contacts in an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "226360c2-5ba0-44ad-815d-4197e4c125d8"
            }
          ]
        },
        {
          "id": "3d0828b5-7389-404e-9a9a-197251565581",
          "name": "getAccountContact_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email"
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given contact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8011f54d-af3c-4cc0-b90b-e547a2fd1dcb"
            }
          ]
        },
        {
          "id": "0b1459ba-29fa-4ad9-a322-1250af1fcca3",
          "name": "listAccountContactFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/files"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists files exchanged with a contact. Returns the latest attachments exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any file attached to an email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "548189ee-4726-46d8-8080-2ae8eabbecb9"
            }
          ]
        },
        {
          "id": "69511c37-d294-4670-a619-2309d95c9d12",
          "name": "listAccountContactMessages_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/messages"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists messages where a contact is present. Returns the latest email messages exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89096296-40fa-419b-a3e7-a208b043ae78"
            }
          ]
        },
        {
          "id": "fb5e064d-71d1-46ef-b22d-65531c4d702a",
          "name": "listAccountContactThreads_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/threads"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists threads where a contact is present. Returns the latest email threads exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56b4d88e-0387-406a-bd16-2d4097a4e4ec"
            }
          ]
        },
        {
          "id": "cb924201-e8d3-4c8d-a6b4-e78604d10062",
          "name": "listAccountEmailAddresses_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists email addresses used by an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3c2f956-d57d-49f8-a3e2-b83963ed0d40"
            }
          ]
        },
        {
          "id": "448f7d21-4141-4288-bf9e-47ab3d260ef8",
          "name": "addAccountEmailAddress_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses"
              ],
              "query": [
                {
                  "key": "email_address",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new email address as an alias for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7ff194d-9f70-4187-b91e-dd5b33f54e84"
            }
          ]
        },
        {
          "id": "24f12088-05ae-4746-aeb7-5d37c27c3f5f",
          "name": "Create_setAccountEmailAddressAsPrimary_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses/:email"
              ],
              "query": [
                {
                  "key": "primary",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Makes this email address the primary one for the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a856155a-5692-49c7-a1bc-b9090f855705"
            }
          ]
        },
        {
          "id": "edd612fc-9430-4160-8bd8-16ede1020728",
          "name": "removeAccountEmailAddress_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses/:email"
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an email address form the aliases of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e60d2ec8-1c65-4065-81ce-03c0ad8e31dd"
            }
          ]
        },
        {
          "id": "e0a306e6-d5f2-4050-9281-803917d1f620",
          "name": "listAccountFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files"
              ],
              "query": [
                {
                  "key": "bcc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "file_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_by_revisions",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists files found as email attachments. List filters: each of the email, to, from, cc and bcc parameters can be set to a comma-separated list of email addresses. These multiple addresses are treated as an OR combination. You can set more than one parameter when doing this call. Multiple parameters are treated as an AND combination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13a61989-c7b3-4408-b8fa-1322a85f73ae"
            }
          ]
        },
        {
          "id": "fb74e618-ab37-4fd0-8895-3f4aa23af543",
          "name": "getAccountFile_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57fa8116-c2c6-4646-a17c-bf6d2bbd36a6"
            }
          ]
        },
        {
          "id": "feab5826-bf2e-4be5-ab24-440c3bb49ece",
          "name": "listComparableAccountFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/changes"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists files that can be compared with a given file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad87e616-ac31-47e2-b9ba-f8d76ab13090"
            }
          ]
        },
        {
          "id": "d3e4aeb1-6aae-4fcb-a74b-6aa7e398957d",
          "name": "getAccountFileContent_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/content"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads a given file. Returns the content a given attachment. On-demand data retrieval: since we do not keep full copies of attachments on our servers, the file has to be retrieved from the IMAP server when this call is made. If the IMAP server is unreachable at the time the call is made, this call will return an error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25a3b0e6-e7b2-4c54-a037-3c730048058b"
            }
          ]
        },
        {
          "id": "67492f0b-ae5c-4dd1-8009-15a8c283a5e3",
          "name": "listAccountFileRelatedFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/related"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists other files related to a given file. Returns a list of files that are related to the given file. Currently, relation between files is based on how similar their names are."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52a7a341-6089-4714-8f1d-ca46339298ca"
            }
          ]
        },
        {
          "id": "1691078f-dabd-42bd-8764-456b0dec7dc1",
          "name": "listAccountFileRevisions_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/revisions"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists other revisions of a given file. Returns a list of revisions attached to other emails in the mailbox for a given file. Two files are considered revisions of the same document if their file names are identical outside of revision indicators such as dates, author initials, version numbers and keywords like \"final\" or \"draft\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0af332a-fb3a-4a53-8c81-126f86aa58f8"
            }
          ]
        },
        {
          "id": "ff05afbd-ed02-4cb5-8d2f-426166b53474",
          "name": "listAccountMessages_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages"
              ],
              "query": [
                {
                  "key": "bcc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "body_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "folder",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_flags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_headers",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subject",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists email messages for an account. List filters: each of the email, to, from, cc and bcc parameters can be set to a comma-separated list of email addresses. These multiple addresses are treated as an OR combination. You can set more than one parameter when doing this call. Multiple parameters are treated as an AND combination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "277d3850-f1ff-49d3-8c06-df6a5c8bf254"
            }
          ]
        },
        {
          "id": "aa1fac32-38a4-4b6b-8fd5-f2c921b4e40e",
          "name": "getAccountMessage_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the file, contact and other information about a given email message. As specified in the RFC822, the < and > at the beginning and end of the Message-ID are part of the value and should be included if you're putting an email_message_id in the url."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2706ce31-0ce8-4643-8484-4afd3568f044"
            }
          ]
        },
        {
          "id": "d8b78e81-8641-483d-8400-2761ca17979c",
          "name": "Create_copyMoveAccountMessage_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id"
              ],
              "query": [
                {
                  "key": "dst_folder",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dst_source",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "move",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Copies or moves a message. Allows you to copy or move a message between folders. If there are more than one sources on the account, you can use this call to copy/move the message between these sources. In this case, the dst_label parameter must identify the source you want to message to be copied/moved to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebba30ed-6f50-42b3-8c0e-4ab26b7773b2"
            }
          ]
        },
        {
          "id": "30476e0a-3755-4963-967b-65e6ffed2e7d",
          "name": "getAccountMessageBody_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/body"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the message body of a given email. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message. One thing to point out is we do fetch messages in such a way that large files attached to a message won't make any difference in the response time. This call only returns text portions of messages, attachments aren't included. To get a list of attachments on the message, look for the files property in the response of a message instance. To download the content of these attachments, use the files/content call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "add7e90c-8728-4db4-8299-31793876e872"
            }
          ]
        },
        {
          "id": "00ef1ad3-b30d-4c26-b321-d405498bb4ce",
          "name": "getAccountMessageSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/source"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the message source. Returns the raw RFC-822 message source for the message (including attachments) with no parsing or decoding to any portions of the message. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message. Attachments are part of the message source so they will impact how fast this call responds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "522c1597-eea4-40a1-b409-d7f833489a57"
            }
          ]
        },
        {
          "id": "2d4d8abb-6289-4bb3-8dba-0dc8ab502ca3",
          "name": "listAccountMessageFlags_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/flags"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists message flags for an account. On-demand data retrieval: to ensure up-to-date values, flags are not cached by Context.IO. This call triggers a connection to the IMAP server to fetch the current message flags before it returns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "468daa39-6253-4281-82be-af95e26c27ab"
            }
          ]
        },
        {
          "id": "61a7c37b-581e-452e-8245-a7b26377adf2",
          "name": "Create_setAccountMessageFlags_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/flags"
              ],
              "query": [
                {
                  "key": "answered",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "deleted",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "draft",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "flagged",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "seen",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets message flags for a given email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9e488b7-5a4a-485f-8312-4e238a39c9ea"
            }
          ]
        },
        {
          "id": "6d05b7e1-3e2e-4d91-b723-9b2e2ff5a158",
          "name": "listAccountMessageHeaders_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/headers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists complete headers of a given email message. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message headers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7893191d-1d15-42f3-8d25-ea944c818819"
            }
          ]
        },
        {
          "id": "7c804153-7fa1-4bca-a687-2e2ac157de8d",
          "name": "getAccountMessageThread_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/thread"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all messages of the thread a given message is in. This returns an array with the same structure as getting information on a single message for every message in the thread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c831eb8f-fb20-4394-a110-c0d8e9224fae"
            }
          ]
        },
        {
          "id": "1a883854-727a-4a84-81f4-847dec7d1aa9",
          "name": "listAccountSources_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources"
              ],
              "query": [
                {
                  "key": "status",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status_ok",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists IMAP sources assigned for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a42bab5-bbe0-4a97-8217-193f5c4200f6"
            }
          ]
        },
        {
          "id": "9746da67-0559-46fd-b200-9d54ba9c8602",
          "name": "addAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources"
              ],
              "query": [
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "port",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_consumer_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token_secret",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "server",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sync_period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "use_ssl",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an IMAP account to a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23d8d8b1-c6e3-42e1-aa9f-53a8dd6b25c3"
            }
          ]
        },
        {
          "id": "a0da8850-13d1-4135-ae53-c1d71e6061cb",
          "name": "getAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "label",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets parameters and status for an IMAP source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5a90a02-2dec-4c44-9272-6ddf32561ab7"
            }
          ]
        },
        {
          "id": "800a8a87-8abe-4d51-abf6-3dbc7048d28f",
          "name": "modifyAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label"
              ],
              "query": [
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_consumer_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token_secret",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sync_period",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "label",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies a data source on a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98040fbf-aea9-40ad-a52b-84551dda2254"
            }
          ]
        },
        {
          "id": "747c666f-eff1-49e7-b0d2-7d4e73d9acec",
          "name": "removeAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "label",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a data source of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2a13561-44e1-4add-b2ba-7a9c9c4b6251"
            }
          ]
        },
        {
          "id": "7fd71629-5c18-4d9c-b50e-1b6cd0b3465e",
          "name": "listAccountSourceFolders_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label/folders"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "label",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists folders in an IMAP source. Returns folders existing in a given IMAP account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33e23538-a4a0-4096-afbd-f085c597bb9b"
            }
          ]
        }
      ]
    }
  ]
}