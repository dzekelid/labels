---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Labels
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Delete Repos Owner Repo Issues Number Labels
  x-api-slug: github
  description: Remove all labels from an issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/labels
  tags: Repos, Owner, Repo, Issues, Number, Labels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-delete-openapi.md
- name: Github Get Repos Owner Repo Issues Number Labels
  x-api-slug: github
  description: List labels on an issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/labels
  tags: Repos, Owner, Repo, Issues, Number, Labels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-get-openapi.md
- name: Github Add Repos Owner Repo Issues Number Labels
  x-api-slug: github
  description: Add labels to an issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/labels
  tags: Repos, Owner, Repo, Issues, Number, Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-post-openapi.md
- name: Github Put Repos Owner Repo Issues Number Labels
  x-api-slug: github
  description: |-
    Replace all labels for an issue.
    Sending an empty array ([]) will remove all Labels from the Issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/labels
  tags: Repos, Owner, Repo, Issues, Number, Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabels-put-openapi.md
- name: Github Delete Repos Owner Repo Issues Number Labels Name
  x-api-slug: github
  description: Remove a label from an issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/labels/{name}
  tags: Repos, Owner, Repo, Issues, Number, Labels, Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabelsname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepoissuesnumberlabelsname-delete-openapi.md
- name: Github Get Repos Owner Repo Labels
  x-api-slug: github
  description: List all labels for this repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/labels
  tags: Repos, Owner, Repo, Labels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabels-get-openapi.md
- name: Github Add Repos Owner Repo Labels
  x-api-slug: github
  description: Create a label.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/labels
  tags: Repos, Owner, Repo, Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabels-post-openapi.md
- name: Github Delete Repos Owner Repo Labels Name
  x-api-slug: github
  description: Delete a label.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/labels/{name}
  tags: Repos, Owner, Repo, Labels, Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabelsname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabelsname-delete-openapi.md
- name: Github Get Repos Owner Repo Labels Name
  x-api-slug: github
  description: Get a single label.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/labels/{name}
  tags: Repos, Owner, Repo, Labels, Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabelsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabelsname-get-openapi.md
- name: Github Patch Repos Owner Repo Labels Name
  x-api-slug: github
  description: Update a label.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/labels/{name}
  tags: Repos, Owner, Repo, Labels, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepolabelsname-patch-openapi.md
- name: Github Get Repos Owner Repo Milestones Number Labels
  x-api-slug: github
  description: Get labels for every issue in a milestone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/milestones/{number}/labels
  tags: Repos, Owner, Repo, Milestones, Number, Labels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepomilestonesnumberlabels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/reposownerrepomilestonesnumberlabels-get-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labels/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---