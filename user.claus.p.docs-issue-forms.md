---
id: ErhsbnmEHZEclL7VTNnxc
title: Docs issue forms
desc: ''
updated: 1643148712563
created: 1643139804748
---

## Research

- [GitHub Docs - Creating issue forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository#creating-issue-forms)
- Prefill issue like `https://github.com/Automattic/wp-calypso/issues/new?labels[]=People%20Management&labels[]=[Type]%20Bug&title=People:&milestone=People%20Management:%20m6&assignee=ebinnion&body=This%20is%20a%20prefilled%20issue`

## WIP

Path `.github/ISSUE_TEMPLATE/documentation.yml`

```yaml
name: Documentation Issue
description: Report a bug in the documentation or suggest a documentation update here
title: "[Docs]: "
labels: ["docs"]
assignees:
  - ryan-p-randall
  - cconrad
body:
  - type: input
    id: ref
    attributes:
      label: Which page/note should be improved?
      description: |
        Unless this is a general issue, please paste a link to the page that your issue is about (or the relative path to the note, or the note ID):
      placeholder: URL or note
      value: 'https://wiki.dendron.so/…'
  - type: textarea
    id: desc
    attributes:
      label: Issue description
      description: |
        **Please describe, as clear and concise as possible, how the documentation can be improved - for example:**
        * Was the documentation incorrect for your/the most recent version of Dendron?
        * Outdated screenshots or movies?
        * Anything that needs to be phrased more clearly?
        * Did the documentation contain invalid usage examples, e.g. missing/renamed commands?
        * Is there something you would like added to the documentation?
    validations:
      required: true
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

- [ ] Check with [foureyedsoul#0796] and [dendronhq] whether assigning both of us by default is fine
- [ ] Uncomment "checkboxes" section when [[Code of Conduct|rfc.39-dendrologists.ref.community-guidelines#future-tasks]] is ready
- Currently, body.ref.value needs to be customized for each repo :/

## Discussion

- Do you agree that OS and versions (of VS Code, Dendron, CLI, node, npm, etc.) may be omitted for this issue type, to simplify the form and improve conversion?
- Which persona do we imagine the typical "docs issue reporter" to have - a Dendron-publishing power user with a multi-vault workspace as well as native ones; a curious manager without admin rights on his device checking out the wiki to find solutions for improving his/her/their teams knowledge sharing; somewhere (where?) in between such extremes?
