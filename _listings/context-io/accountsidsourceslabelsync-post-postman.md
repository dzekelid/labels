{
  "info": {
    "name": "Context.IO Post Accounts Sources Label Sync",
    "_postman_id": "15ba49d7-3f60-4587-ba68-cd7e38fde1f9",
    "description": "Triggers a sync of a data source. This will start a sync job for the source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "75f21eda-916a-45d3-a572-c061a7018456",
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
              "id": "961f5b8e-6941-461a-86a2-18712e21970f"
            }
          ]
        },
        {
          "id": "ddd2aee3-d87d-41e9-893d-fea848d14669",
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
              "id": "81f34fe8-0308-4e04-bd44-b4fbf78a1bbf"
            }
          ]
        },
        {
          "id": "91ed7b78-d265-42b4-9842-4d16b23e6bdd",
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
              "id": "1b255c22-211c-404e-9489-fc563a709cfa"
            }
          ]
        },
        {
          "id": "ad55e0f5-c7e4-42e4-8119-b952dd019983",
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
              "id": "66a357ee-61b0-4b9e-b7e1-fb2834fc5217"
            }
          ]
        },
        {
          "id": "45a6d82d-0d2e-4892-9060-7cf12a5a5c75",
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
              "id": "4c969b30-ef06-4997-99d4-224381072fa9"
            }
          ]
        },
        {
          "id": "cc142ffb-0cba-4b93-8c9a-f8281ece5e65",
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
              "id": "e3661c99-c2b5-4f60-b167-cf3a246d85f9"
            }
          ]
        },
        {
          "id": "aef5538e-2d41-42c2-b738-05f4466bd263",
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
              "id": "c5c55838-19da-456f-842e-b736fd0e0ac1"
            }
          ]
        },
        {
          "id": "ceaf4cf7-b63c-40b7-b312-2999b909dc38",
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
              "id": "85e88454-67a1-4e46-afc7-e39d5160a6ff"
            }
          ]
        },
        {
          "id": "8137a3db-e107-4a40-b9f6-051909c5970f",
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
              "id": "45928d51-a02b-44c8-969e-14a30c1337eb"
            }
          ]
        },
        {
          "id": "ce9ef464-721b-43c3-ab26-40c80234ef1d",
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
              "id": "ed36ba6b-9df4-4684-93fb-98a75c6cede6"
            }
          ]
        },
        {
          "id": "022dd380-9d8c-416e-9f8a-7a669171ffb6",
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
              "id": "60602b3e-abb4-41a6-b4bd-bf45d898fcbb"
            }
          ]
        },
        {
          "id": "4480517b-ea18-4dad-a173-f95b331add2b",
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
              "id": "f7418801-8704-4869-b859-4f22a4892ccb"
            }
          ]
        },
        {
          "id": "01ad1115-f723-42b9-adc1-b462d0f7bdda",
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
              "id": "f8294ce2-668c-4f07-b8b3-52132518dde3"
            }
          ]
        },
        {
          "id": "0f49dc6c-3098-414f-ae99-ec32d2221ab7",
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
              "id": "7686791f-6584-4774-bbc0-83745d8072d1"
            }
          ]
        },
        {
          "id": "af6d6787-3b67-4149-af4b-e358af2945a5",
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
              "id": "674e9c7c-2f6f-4603-a2b9-f4213c248168"
            }
          ]
        },
        {
          "id": "e97fbb25-f165-4e2f-8489-52d869c8573a",
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
              "id": "16578054-3596-40fd-b66c-140794dfeefd"
            }
          ]
        },
        {
          "id": "ccc10bdb-cfbd-4115-a3c2-cf8eef7f9e65",
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
              "id": "af432c14-72bd-4f2d-81ca-8e0fda0e2b07"
            }
          ]
        },
        {
          "id": "f565e387-9767-4b74-bb40-632fcce7bcc0",
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
              "id": "12568cc9-cdef-4cc3-b1b5-a87a36beaf5c"
            }
          ]
        },
        {
          "id": "1712bb2d-9e84-41b9-a881-824234d61f1f",
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
              "id": "f681e2e5-4d5d-4d3b-9306-b0b09b0a6049"
            }
          ]
        },
        {
          "id": "e4fab134-d176-4c90-ae0d-6d8c497121fd",
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
              "id": "3a92a46a-b3ae-4f74-94ba-f7516640dd97"
            }
          ]
        },
        {
          "id": "568fa3a3-44b2-447a-94b5-25af47a17f5b",
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
              "id": "36470246-8029-4b62-9b34-20da5be5d370"
            }
          ]
        },
        {
          "id": "a3eaee38-f8eb-4abd-839c-7e50d8648e05",
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
              "id": "f9f209f1-a875-4fa5-a3c9-0f45ae71b303"
            }
          ]
        },
        {
          "id": "fd86e815-9fa0-4aed-97a7-732327063f9e",
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
              "id": "5012cf8e-1352-42b1-9985-56ee9a63c3ae"
            }
          ]
        },
        {
          "id": "1ec99dfe-2dce-42a0-a8b2-859ae20637f4",
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
              "id": "ab0083a6-edfe-4e54-8dbf-cb675af67bb9"
            }
          ]
        },
        {
          "id": "f2c31f58-40eb-4c6d-8613-f4dcbca245fc",
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
              "id": "b6f7ec32-03cf-4c04-a1e2-3ca3a86c0c63"
            }
          ]
        },
        {
          "id": "3f778b24-4058-4d57-94a8-c939b77effdc",
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
              "id": "ded3d7e2-04e0-4c11-b05a-a9efb25df136"
            }
          ]
        },
        {
          "id": "229fb9f6-b3d5-4663-8e79-71d61d8cac47",
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
              "id": "82ad6505-d1a9-40f6-8d5e-7e0d61150917"
            }
          ]
        },
        {
          "id": "86065d15-ca77-4fb7-8364-5fddf090aee3",
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
              "id": "6a389574-7608-473d-a9fe-7b8b8aadf5a3"
            }
          ]
        },
        {
          "id": "9d825d84-bad3-4d5f-b73f-40fc059e94ce",
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
              "id": "00253952-0a65-49ac-9798-f9b05c25c865"
            }
          ]
        },
        {
          "id": "d75c309b-78c7-423f-986a-a22b5703b74a",
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
              "id": "489516d8-2698-4bee-aebf-87a66f26070f"
            }
          ]
        },
        {
          "id": "39449a6a-5cf4-4468-b639-51c0989d53fe",
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
              "id": "f2ecb210-10e0-4111-b32a-4fc4c7da3f84"
            }
          ]
        },
        {
          "id": "0538ac4c-c8cd-4fea-a306-8810aaf835ce",
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
              "id": "f184998d-e792-4a11-9a1f-7ffd8db13252"
            }
          ]
        },
        {
          "id": "cc2f809e-6428-46f3-a540-c58a95ab5b95",
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
              "id": "d87bb154-2edb-4d28-bfc4-54a94913bd1f"
            }
          ]
        },
        {
          "id": "cd0423a8-668b-4638-b353-811ecbf942dc",
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
              "id": "64e3e988-a9c1-463a-b539-cd4d6d4a5fbd"
            }
          ]
        },
        {
          "id": "ae5bcef6-b6cb-43f5-9f8c-f3f78b30ab0d",
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
              "id": "5e77ccc8-435c-477b-ad31-96c7d362d27a"
            }
          ]
        },
        {
          "id": "2a1b4483-48fc-4f0f-84c7-30ef0fc4f777",
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
              "id": "b4c21774-4d36-401d-80b4-8db247f6741d"
            }
          ]
        },
        {
          "id": "038d5b98-26e8-478b-af06-eae2df73e67d",
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
              "id": "58f9001f-090c-430e-bc52-e409f6a80b75"
            }
          ]
        },
        {
          "id": "035670b6-d1a9-4ca4-bf49-9975d9dde60c",
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
              "id": "dae97817-d3a5-4fc2-a937-a9b566bb5344"
            }
          ]
        },
        {
          "id": "9f7e7a0f-eec4-4965-b9b1-7b80215fabe6",
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
              "id": "9b7acd68-c564-4562-a909-b42a9a76016b"
            }
          ]
        },
        {
          "id": "e7de4270-c78c-402b-8229-24ee2e67b304",
          "name": "createAccountSourceFolder_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label/folders/:folder"
              ],
              "query": [
                {
                  "key": "delim",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "folder",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Creates a folder on an IMAP source. A new folder can be added to an IMAP source by PUTting the desired path under the sources/folders resource.\nWorking with server-specific hierarchy delimiters:\nIMAP servers are free to use the character they want as the folder hierarchy delimiter. The bad news is they don't use the same. The good news is you don't need to know this, we take care of it.\n\nThen what is that delim parameter for?\nGood question. By default, we expect you to specify the folder hierarchy using / as the hierarchy delimiter. For example, to create a folder called my folder under the folder base folder, you would call:\nPUT /2.0/accounts/<id>/sources/<label>/folders/base+folder/my+folder\n\nNo matter what's the actual hierarchy delimiter the IMAP server expects, this call will work. However, say you need to use another character as the delimiter, here's how you'd do it:\nPUT /2.0/accounts/<id>/sources/<label>/folders/base+folder.my+folder?delim=.\n\nBoth examples above are equivalent and will have the same result no matter what the IMAP server expects as the actual hierarchy delimiter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "714a497e-9d2b-4867-b1b4-65022db3490b"
            }
          ]
        },
        {
          "id": "d95f4c1c-e0d1-4afd-9c2c-e639e50f09b9",
          "name": "getAccountSourceSyncStatus_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label/sync"
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
            "description": "Gets the sync status of a data source. Returns the timestamps for the last time the source has been synced with the origin mailbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f9f2a60-8dd3-4612-970e-28e6b9d83cf3"
            }
          ]
        },
        {
          "id": "a54fe60f-84af-4732-b106-ce94224e0ef0",
          "name": "Create_syncAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources/:label/sync"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Triggers a sync of a data source. This will start a sync job for the source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e6d1c9d-d737-4c32-9b9c-0dfc89d3f3d7"
            }
          ]
        }
      ]
    }
  ]
}