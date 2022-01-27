---
id: 9hQj6ySoRsLTC2oIrpDjv
title: Create PR Templates for Docs Repos
desc: ''
updated: 1642730191102
created: 1642726212000
tags:
  - scope.docs
  - type.chore
  - sprint
  - kind.focus.docs
  - size.medium
status: ''
due: ''
priority: ''
owner: ''
creator: derek
issue: ''
pr: ''
card: 'https://github.com/orgs/dendronhq/projects/9#card-76441503'
airtableId: reccJKjTiPuKyGMKL
---

## Summary

Our primary code repository, [dendronhq/dendron](https://github.com/dendronhq/dendron), has a PR template in place. We should have standard, baseline PR templates for each of our docs repos. A `CONTRIBUTING.md` should also exist within each repository.

## Details

### Generic docs PR template

Something at least including the following:

```markdown
## What does this PR do?
<!-- Describe pull request here. -->

## What issues does this PR fix or reference?

- Resolves:
OR
- Relates to:

(Resolve will close the ticket after merging. Relate will leave the ticket open
after merging.)

### Merge requirements satisfied?

> For more information, visit the [Contributing Guide for Documentation](https://wiki.dendron.so/notes/b58801fc-43a9-4d42-a58b-eabc3e8538cb/)

- [ ] Check rendered output to ensure formatting is correct for renderings of wikilinks, note refs, tables, and images. `Dendron: Show Preview` can be used in your workspace to confirm the page renders as expected. Sometimes, `Dendron: Reload Index` needs to be ran if certain wikilinks aren't working as expected. (ignore this if contribution is made via the `Edit this page on GitHub` button from the published site)

Verify GitHub Actions tests are passing, which can be seen in the `Checks` tab of the PR:

- [ ] `URL validator` GitHub Action passes
- [ ] `Dendron site build` GitHub Action passes

> If you are a new contributor, a maintainer will need to provide approval for GitHub Actions to run on your PRs.
```

> Modify the `Merge requirements satisfied?` section, depending on what is required for the target repository

## Example

- Example docs PR templates
  - [salts basic docs MR template](https://gitlab.com/saltstack/open/docs/salt-user-guide/-/blob/master/.gitlab/merge_request_templates/salt-user-guide-merge-request.md)
- Example of links instead of issue templates (such as when users are asking for help)
  - [saltstack/salt: config](https://github.com/saltstack/salt/blob/master/.github/ISSUE_TEMPLATE/config.yml)

## Tasks


## Lookup
- [About community profiles for public repositories](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/about-community-profiles-for-public-repositories)
- [Open Source Guides](https://opensource.guide/)
