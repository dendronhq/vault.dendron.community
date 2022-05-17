---
id: ebpudfrf6rg5uut75d29lhg
title: Standard Documentation
desc: ''
updated: 1652803408417
created: 1651791209320
documentId: 1DD6ROb22u-BpLeSY_WUlqedMqVCI25wm-gB6EXw0liI
revisionId: >-
  ALm37BVgmvBsP9mZcAMWNpdo8kdYFF4EfvXim0OXn9y_CcP0iLP1id9x06TJiv-P2tGeWo7QAme-uZC13lXULA
---

## Summary

This leaflet proposes some general guidelines for the Dendron public docs for the following purposes:
- make it umnabiguous where to add howtos/reference/discussions/tutorials on new features and capabilities
- make it umnabiguous where to find howtos/reference/discussions/tutorials on existing features and capabilities
<br/>
- NOTE: this doc is generated from [[Standard Documentation|dendron://dendron.community/leaflet.journal.2022.05.10.standard-documentation]]

## Concepts
For the purposes of this discussion, howtos/reference/discussions/tutorials refer to the [four types of documentation](https://kevinslin.com/notes/y0swab2mazgi1793kp3v7f7)

## Details

There are two areas that this leaflet addresses. 
- the **overall structure** of the docs 
- the **structure for features** 

## Overall Structure of Docs

This leaflet proposes the following changes:

- simplify user guide (less children)
- simplify dendron.* hierarchy to be product related topics 
    - make contribution its own top level hierarchy
- rename "Guides" to "How tos" 

Resulting hierarchhy:

- dendron
    - dendron.quickstart (Getting Started)
    - dendron.user-guide (User Guide)
        - Basic
        - Edit
        - Retrieve and Navigate 
        - ~~Navigation~~ 
            - > fold into Retrieve
        - ~~Organize~~ Structure 
            - > Rename to `Structure`
        - ~~Refactoring~~ 
            - > Fold into `Structure`
        - Sharing and Syncing
        - ~~Transferring~~ 
            - > Rename to `Sharing and Sncing`
        - Extending
    - ~~dendron.principles~~  
        - > fold into `dendron` home page
    - ~~FAQ~~ 
        - > move under `dendron.res`
    - ~~dendron.contribute~~
        - > move to `contribute` (becomes top level hierarchy)
    - ~~dendron.guides~~
        - > Rename to `dendron.howtos` (How)
    - dendron.concepts (Concepts)
    - dendron.ref (Reference)
    - dendron.res (Resources)
        - dendron.res.faq
        - dendron.res.troubleshooting
        - dendron.res.support
- contribute 
    - > everything from dendron.contribute gets moved here
- community
- changelog
- careers

## Structure for Features

All features today lie are added in the form `dendron.topic.{feature}`

### Sections

These are heades for features and are directly inside `dendron.topic.{feature}`

```md
## Summary
<!-- 
- recommended: include a picture
- eg: [[Summary|dendron://dendron.dendron-site/dendron.topic.publish#summary]]

3 sentence description of the feature
-->

## Use Cases
<!--
Bullet points with examples of how this feature could be used
-->

## Features
<!-- 
- required: false
- example: [[Features|dendron://dendron.dendron-site/dendron.topic.publish.features]]

If the feature has sub features, list them out here 
-->

### Limitations
<!-- Optional. If there are any limitations to call out -->

## Getting Started
<!-- 
- eg: [[Quickstart|dendron://dendron.dendron-site/dendron.topic.publish.quickstart]]

How to get started using the feature. Should have a link to the quickstart doc
-->

### Child Pages
<!-- 
Link to children 

Should have following order

- Concepts
- Config
- CLI
- Commands
-->
```

### Children
These are the children of features and are located in `dendron.topic.{feature}.*`

- values in orders:
    - quickstart: how to start using the feature (this is what is linked to under `Getting Started`)
    - concepts: concepts this feature introduces
    - config: relevant configuration
    - cli: relevant cli
        - eg: [[CLI|dendron://dendron.dendron-site/dendron.topic.publish.cli]]
    - commands: commands in the page
    - details: internal details about how the feature works
    - migration: how to migrate (if applicable)
    - faq: frequently asked questions
    - tutorials
    - howtos


For `concepts`, `config`, `cli`, `commands`, the proposal is to have each individual `concept/config/cli/command` be a separate note. This makes it easy to refer to individual entities by themselves. See [[Configuration|dendron://dendron.dendron-site/dendron.topic.publish.config]] for an example
