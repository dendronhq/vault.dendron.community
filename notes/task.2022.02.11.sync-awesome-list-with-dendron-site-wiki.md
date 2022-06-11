---
id: uu1gE6PTg3EPDxCwB1naf
title: Sync Awesome List with Dendron Site Wiki
desc: ''
updated: 1645073806274
created: 1644617106749
tags:
  - scope.growth.community
  - type.doc
  - sprint.backlog
  - kind
  - size.big
status: ''
due: ''
priority: ''
owner: derek
creator: derek
issue: ''
pr: ''
userIssueId: ''
airtableId: rec2qtGRG0BRqWST9
---

## Summary

GitHub Actions should be used to sync [`awesome-dendron`](https://github.com/dendronhq/awesome-dendron/) with a note inside of [`dendron-site`](https://github.com/dendronhq/dendron-site).

## Details

`awesome-dendron` content should be used to replace:

- [[Extensions|dendron://dendron.dendron-site/dendron.topic.extensions]]
- [[Other VS Code Extensions|dendron://dendron.dendron-site/dendron.guides.tips#other-vs-code-extensions]]

It might make the most sense to:

- Create `dendron.guides.awesome-dendron` (or similar?)
- Update the existing notes to become note refs of content existing inside of `awesome-dendron`
- Existing notes should include a note that if they want to contribute to the page, that they should contribute to the `awesome-dendron` repo instead since it is the source
- Use `canonicalUrl` inside of the page created in `dendron-site` to point to the `awesome-dendron` repo

## Example

## Tasks

## Lookup
