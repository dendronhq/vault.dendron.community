---
id: ErhsbnmEHZEclL7VTNnxc
title: Docs issue forms
desc: ''
updated: 1644346503730
created: 1643139804748
---

## Research

- [GitHub Docs - Creating issue forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository#creating-issue-forms)
- [Prefill form](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue#creating-an-issue-from-a-url-query) like `https://github.com/octo-org/octo-repo/issues/new?labels=bug&title=New+bug+report`

## WIP

Path `.github/ISSUE_TEMPLATE/documentation.yml`

```yaml
name: Documentation Issue
description: Report a bug in the documentation or suggest a documentation update here
labels: ["docs"]
assignees:
  - ryan-p-randall
  - cconrad
body:
  - type: input
    id: ref
    attributes:
      label: Which docs page should be improved?
      description: "Unless this is a general issue, please paste a link to the page that it is about:"
      placeholder: URL (or note ref)
      value: "https://wiki.dendron.so/…"
  - type: checkboxes
    id: action
    attributes:
      label: Which area does your issue apply to?
      description: Multiple selections are possible - leave blank if unsure.
      options:
        - label: 'Basics: Fundamental Dendron features, installation, getting started etc.'
        - label: 'Editing: Editing your notes, Markdown, frontmatter, images, templates, links, note refs, etc.'
        - label: 'Retrieving: Finding your notes, lookup, lookup modifiers, etc.'
        - label: 'Navigating: Navigating across notes, graph view, go to shortcuts, etc.'
        - label: 'Organizing: Maintaining your notes, hierarchies, schemas, journals, tags, users, tasks, special notes, vaults, workspaces, multi-vault, etc.'
        - label: 'Refactoring: Restructuring your notes, Dendron Doctor, refactor hierarchy, move/rename notes, rename header, etc.'
        - label: 'Sharing: Publishing and sharing your notes, git, team workflows, etc.'
        - label: 'Transferring/syncing: Importing/exporting your notes, pods, etc.'
        - label: Extending note and workspace functionality, note type system, note traits, hooks, custom pods, etc.
        - label: Dendron community
        - label: Other (please describe in the issue description below)
  - type: checkboxes
    id: area
    attributes:
      label: What should be fixed/improved?
      description: Multiple selections are possible
      options:
        - label: Fix outdated docs
        - label: Extend docs (tutorials, workflows, etc.)
        - label: Add docs (new features, etc.)
        - label: Clarification needed
        - label: Add/update screenshots
        - label: Fix broken formatting, wikilink, and/or note references
        - label: Other (please describe in the issue description below)
  - type: textarea
    id: desc
    attributes:
      label: Issue description
      description: |2
        **Please describe, as clear and concise as possible, where the documentation can be improved - for example:**
        * Was the documentation incorrect for your/the most recent version of Dendron?
        * Outdated screenshots or movies?
        * Did the documentation contain invalid usage examples, e.g. missing/renamed commands?
        * Feel free to attach screenshots
    validations:
      required: true
  - type: textarea
    id: suggestion
    attributes:
      label: Suggested fix, improvements or additions
      description: |2
        **Please describe, as clear and concise as possible, if you have suggestions on how the issue can be solved - for example:**
        * Anything that needs to be phrased more clearly?
        * Is there something you would like added to the documentation?
#  - type: checkboxes
#    id: terms
#    attributes:
#      label: Code of Conduct
#      description: Our [Code of Conduct]() helps create a safe space for everyone.
#      options:
#        - label: I agree to follow the Dendron Community Code of Conduct
#          required: true
  - type: markdown
    attributes:
      value: |
        Thank you for taking your time to help improve Dendron's documentation! 🌱
```

## Issues

- [x] Check if issue titles on dendronhq/dendron have prefixes (e.g. "[Bug]: ")
- [ ] Test if the colons make sense in the UI
- [ ] Check with [foureyedsoul#0796] and [dendronhq] whether assigning both of us by default is fine
- [ ] Uncomment "checkboxes" section when [[Code of Conduct|rfc.39-dendrologists.ref.community-guidelines#future-tasks]] is ready
- Currently, body.ref.value needs to be customized for each repo :/
- JavaScript 

## Discussion

- Do you agree that OS and versions (of VS Code, Dendron, CLI, node, npm, etc.) may be omitted for this issue type, to simplify the form and improve conversion?

  > good for me

  - Source <https://discord.com/channels/717965437182410783/933936685832601770/935670943232188447>

- Which persona do we imagine the typical "docs issue reporter" to have - a Dendron-publishing power user with a multi-vault workspace as well as native ones; a curious manager without admin rights on his device checking out the wiki to find solutions for improving his/her/their teams knowledge sharing; somewhere (where?) in between such extremes?

  > good question. might be good to scan past docs PR to get a sense. also wouldn't necessarily bias towards that (we want to make it simpler for folks to either directly contribute docs or make suggestions so making it easier for more people). that being said, about 50% of our user base is developers  so that's a good starting point
  
  - Source <https://discord.com/channels/717965437182410783/933936685832601770/935670943232188447>

## Feedback

> also, not saying at all we need to do this for docs - when creating issues for dendron, we have this template: https://github.com/dendronhq/dendron/blob/master/.github/ISSUE_TEMPLATE/feature_request.md#L13:L13
>
> we also have an issue labeler that attaches labels. is it worthwile to do that for docs? if so, feel free to use the above as a starting point

- Source <https://discord.com/channels/717965437182410783/933936685832601770/935671396015673404>

> Would an issue template with that information lead to too much cognitive load? Or would it ultimately be more helpful over time?

- Source <https://discord.com/channels/717965437182410783/933936685832601770/935946154363985983>
