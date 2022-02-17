---
id: W0cG2ju8J1cKT0wdt4o2s
title: wikilinkToURLs and Publishing Vault Configurations
desc: ''
updated: 1645130784238
created: 1645130003031
tags:
  - scope.publish
  - type.feature
  - sprint
  - kind
  - size
status: ''
priority: ''
owner: ''
creator: derek
issue: ''
pr: ''
userIssueId: ''
airtableId: recuMzBUGthsUCoMn
---

## Summary

Support mappings of site URLs to cross-vault notes.

## Details

When publishing our docs sites, such as `dendron-docs` and `dendron-site`, cross-vault note references get converted to red private links. This makes certain areas of our documentation only useful when using workspaces that include the seeds being referenced.

If publishing configurations could support mappings of site URLs to cross-vault notes, this would make publishing more powerful.

## Example

- `dendron.dendron-docs` has a known siteUrl of `https://docs.dendron.so`
- `dendron.dendron-site` has a known siteUrl of `https://wiki.dendron.so`

Both workspaces contain this information within their `dendron.yml`.

If the `dendron.dendron-site` workspace could include the `dendron.dendron-docs` as a seed, that is exempt from publishing, it would be useful for all cross-vault references to `dendron.dendron-docs` notes to be converted to the proper external website link. Having `dendron.dendron-docs` as a seed should mean that `dendron.dendron-site` would be able to:

- See the `siteUrl` for `dendron.dendron.docs`
- See the addociated Dendron ID of the notes being referenced
- Use the combination to create external URLs without them needing to be Private Links

> NOTE: The design and implementation of this feature may be impacted by [[RFC 42 Self Contained Vaults|dendron://dendron.docs/rfc.42-self-contained-vaults]]. Though, if a vault included in a dependency contains a `siteUrl` within the `dendron.yml` of the dependency vault, it would be feasible to have some configuration at the top-level vault `dendron.yml` that opts to use the `siteUrl` for all cross-vault links to specific vault dependencies. This would allow targeted conversion of link, while leaving other untargeted links as usual Private Links upon publishing.

## Tasks

## Lookup
