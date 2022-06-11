---
id: 4L3dPOvgfcLHx92YKBMRU
title: Dendron Site Reorganization
desc: ''
updated: 1636580024034
created: 1636073824334
category: RFCs/Ideas
discussionID: D_kwDOEF_3Vs4AN_-L
url: 'https://github.com/dendronhq/dendron/discussions/1665'
author: 'https://github.com/dendron-bot'
---

# Summary

This is divided into two parts.

1. **Site Organization** is how the new site should be organized
2. **Other Things** contains other proposals and feature proposals to make the site easier to use

- NOTE: this discussion is available in [[Dendron Site Reorganization|dendron://private/proj.2021-11-dendron-site-reorg.v1]] inside the Dendron team workspace.

## Tags
- #later: means this will be done at a later phase and won't be part of the initial migration


# Site Organization

## Top Level Hiearchy
```
- Dendron
    - Getting Started (dendron.tutorial)
        - ...
    - User Guide (dendron.user-guide)
        - Basics 
        - Editing 
        - Retrieving 
        - Organizing 
        - Sharing 
        - Transferring 
        - Extending 
    - FAQ (dendron.faq)
        - Editing
        - Retrieving
        - Organizing
        - Sharing
        - Transferring
        - Extending
        - Alternatives
    - Guides (dendron.guides)
        - Cookbook
        - Troubleshooting
        - Workflows 
    - Concepts
    - Contribute
    - Careers
    - Reference
        - CLI: contains all CLI commands
        - Configuration: all configuration
        - Commands: all commands
        - Features: all features (topics)
        - Dendron Maturity Levels (dendron.ref.maturity)
        - Telemetry: Our telemetry notice
- Changelog
    - v0.6x
    - v0.x
    - ...
- Community 
    - ...
- Tags
```

### Details
- Getting Started: linear tutorial
- User Guide: all current topics arranged by area. All areas are actions that are related to notes
    - Basics: fundamental core features of Dendron 
    - Editing
    - Retrieving
    - Organizing
    - Sharing
    - Transferring: move notes to other places (pods)
    - Extending: extending Dendron (note type system, custom pods, hooks)
- FAQ: frequently asked questions, made up of note references pointing to existing features
- Guides: walkthroughs 
- Concepts: definition of terms, made up of note references pointing to existing features
- Contribute: how to contribute to Dendron
- Careers: jobs page
- Reference: an appendix to lookup specific information

## User Guide

### Basics
```md
- [[Lookup|dendron://dendron.dendron-site/dendron.topic.lookup]]
- [[Hierarchies|dendron://dendron.dendron-site/dendron.topic.hierarchies]]
- [[Markdown|dendron://dendron.dendron-site/dendron.topic.markdown]]
- [[Images|dendron://dendron.dendron-site/dendron.topic.images]]
- [[Links|dendron://dendron.dendron-site/dendron.topic.links]]
- [[References|dendron://dendron.dendron-site/dendron.topic.note-reference]]
- [[Templates|dendron://dendron.dendron-site/dendron.topic.templates]]
- Journals (todo: split out into own section)
- [[Workbench|dendron://dendron.dendron-site/dendron.topic.workbench]]
- [[Graph View|dendron://dendron.dendron-site/dendron.topic.graph-view]]
```

### Editing Notes
- [[Frontmatter|dendron://dendron.dendron-site/dendron.topic.frontmatter]]
- [[Note References|dendron://dendron.dendron-site/dendron.topic.note-reference]]
- Math and Diagrams

### Retrieving Notes
- [[Lookup Modifiers|dendron://dendron.dendron-site/dendron.topic.lookup.modifiers]]
- [[Lookup Keybindings|dendron://dendron.dendron-site/dendron.topic.lookup.keybindings]]
- Search? (don't currently have a note on this)

### Organizing Notes
- [[Schemas|dendron://dendron.dendron-site/dendron.topic.schema]]
- Builtin Note Types(todo: create)
    - [[Tags|dendron://dendron.dendron-site/dendron.topic.tags]] 
    - [[Users|dendron://dendron.dendron-site/dendron.topic.users]]
    - [[Tasks|dendron://dendron.dendron-site/dendron.topic.tasks]]
    - [[Special Notes|dendron://dendron.dendron-site/dendron.topic.special-notes]]
- [[Vaults|dendron://dendron.dendron-site/dendron.topic.vaults]]
- [[Workspace|dendron://dendron.dendron-site/dendron.topic.workspace]]
- [[Multi Vault|dendron://dendron.dendron-site/dendron.topic.multi-vault]]

### Sharing Notes
- [[Git|dendron://dendron.dendron-site/dendron.topic.git]]
- [[Publish|dendron://dendron.dendron-site/dendron.topic.publish]]
- [[Teams|dendron://dendron.dendron-site/dendron.topic.teams]]

### Transferring Notes
- [[Pods|dendron://dendron.dendron-site/dendron.topic.pod]]

### Extending Notes
- Note Type System (todo)
- [[Hooks|dendron://dendron.dendron-site/dendron.topic.hooks]]
- Custom Pods (todo)

## Feature Anatomy

A feature is represented as `dendron.topic.*`.
Every topic is a feature with the following template

```md
## Summary
<!-- 3 sentence description of the feature -->

## Details
<!-- In depth explanation of feature -->

## Concepts
<!-- Concepts that relate particular topic-->

## Examples
<!-- showcase sample use cases -->

## Commands
<!-- VSCode specific commands if applicable -->

## CLI
<!-- cli specific commands if applicable -->

## Config
<!-- configuration if applicable -->

## FAQ
<!-- Commonly asked questions -->

## Cookbook
<!-- Commonly used commands -->

## Troubleshooting
<!-- Common errors -->
```

If a feature has subfeatures, they should be a child of the topic and show up under children. 

## FAQ

Every feature has its own FAQ in its own hierarchy. The FAQ note has note references into each topic. These note references are grouped in the same way as the `User Guide`

In adition, it also has some specific questions that are not feature related  (eg. Dendron Alternatives)

## Guides

Guides on how to do specific things

- Cookbook: compiled from note reference of all features [^1]
- Troubleshooting: compiled from note reference of all features
- Workflows: manually written tutorials on common workflows (eg. zettelkasten, bullet journal, etc)
    - move notes from [[dendron.case-studies]]

## Concepts

Compiled from note reference of all feature

## Contribute

Same as today. Group by [[mark suggestion|dendron://private/user.hikchoi.scratch.2021.10.30.site-reorg#dendroncontribute]]

## Careers

This is the `dendron.jobs` page 

## Reference

The reference section is an appendix of everything. It is a horizontal slice across all features.

- CLI: compiled from note reference of all features
- Configuration: compiled from note reference of all features
- Commands: compiled from note reference of all features
- Features: link to all features
- Dendron Maturity Levels (dendron.ref.maturity)
- Telemetry: Our telemetry notice

## Changelog

Same as current

## Community

Same as current

## Tags

Same as current

***

# Other Things

## More useful Schemas
#later

- See [[Jonathan schema comment|dendron://private/scratch.2021.10.27.212301.jonathan-dendron-site-remap#^GVdwkabWPsUf]]
- We should make schemas more useful (eg. click on a schema to get an overview of what it covers) in published pages (or remove them if they are not useful)

## Admonitions
#later

- we should use the following to indicate special information

- NOTE: an important detail that should be taken into account
- TIP: something that will make 
- WARNING: a potentially destructive action

## Content Migration

The following notes should be migrated to a different domain
- move to `docs.dendron.so`
    - `pkg.*` 
    - `dendron.rfc.*`

## Landing Page additions

- merge notes from [[dendron.features]] here
- move [[dendron.testimonials]] to landing page

## Tasks
- plug onboarding and open pkm at the end of tutorial

- remove
    - dendron.blog
    - templates
    - dendron.cheatsheet
    - dendron.discussion
- rename
    - dendron.topic.references -> dendron.topic.note-reference
    - dendron.release -> dendron.changelog
- move
    - dendron.topic.math >> dendron.topic.math-and-diagram
    - dendron.topic.markdown#mermaid >> dendron.topic.math-and-diagram

## 

[^1]: this means taking a note reference of the same section from each feature of Dendron if it exist. you can see the sections within each feature in [[Feature Anatomy|dendron://private/proj.2021-11-dendron-site-reorg.v1#feature-anatomy]]. Unless otherwise stated, the note references will be grouped by action (see user guide). Not all features will have a note reference for each section.
