---
id: 8JNdYpnY42nFY8minwez9
title: Create Issue Templates for Docs Repos
desc: ''
updated: 1642725959521
created: 1642724623791
tags:
  - scope.admin
  - type.doc
  - sprint
  - kind.focus.docs
  - size.medium
status: 'released'
owner: 'derek'
creator: derek
pr: 'https://github.com/dendronhq/dendron-site/pull/404'
card: 'https://github.com/orgs/dendronhq/projects/9#card-76437321'
airtableId: recIlYuInIHFmxHlS
---

## Summary

Our primary code repository, [dendronhq/dendron](https://github.com/dendronhq/dendron), has issue templates in place. We should have standard, baseline issues for each of our docs repos along with helpful links for users wanting to ask questions (such as links to our Discord).

## Details

> Use [GitHub Issue Forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository#creating-issue-forms) where possible, whenever creating issue templates in Dendron GitHub repos

### Generic docs issue template

Contents:

- Describe the docs issue
- Link(s) to documentation
- Suggested fix, improvements, or additions
- Optional: If applicable sections
  - Versions
    - OS
    - VS Code (or VSCodium) Version
    - Dendron Extension Version
    - CLI Version
      - Node.js / npm versions

### Basic config for optional paths

Contents:

- Dendron Community
  - "For troubleshooting, general questions, and community involvement"
  - Link: https://wiki.dendron.so/notes/6f4cd441-f883-4e75-871b-b7f93895c91b/
- Dendron GitHub Discussions
  - "View Requests For Comment (RFC) discussions, community queries, and more in our discussions."
  - Link to the `dendronhq/dendron/discussions`

## Example

- Existing issue experience in [dendronhq/dendron](https://github.com/dendronhq/dendron/issues/new/choose)
  - [Templates](https://github.com/dendronhq/dendron/tree/master/.github/ISSUE_TEMPLATE)
- Example docs templates
  - [saltstack/salt: docs](https://github.com/saltstack/salt/blob/master/.github/ISSUE_TEMPLATE/docs.md)
- Example of links instead of issue templates (such as when users are asking for help)
  - [saltstack/salt: config](https://github.com/saltstack/salt/blob/master/.github/ISSUE_TEMPLATE/config.yml)

## Tasks

- [GitHub PR](https://github.com/dendronhq/dendron-site/pull/404)
- Completed: [`documentation.yml`](https://github.com/dendronhq/dendron-site/blob/master/.github/ISSUE_TEMPLATE/documentation.yml)
  - Experience: [New `dendron-site` issue](https://github.com/dendronhq/dendron-site/issues/new/choose)

## Lookup

