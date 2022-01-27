---
id: xG06XjLbPH1yn03rOT5dE
title: Root
desc: ''
updated: 1643253544688
created: 1643046665282
---


# Welcome to the Dendron Community Vault

To setup this workspace, clone the following repository

```sh
git clone git@github.com:dendronhq/ws.dendron.community.git
# open up the `dendron.code-workspace` file
```

This will also give you an idea of what its like to work collaboratively in Dendron. We'll be following the exact same process that we do internally in the team.

When you open the workspace with Dendron, it will pull down the following vaults:

- dendron.community (what will become the dendron community site and where we will coordinate on SOPs and initiatives)
- dendron.dendron-site: https://wiki.dendron.so/
- dendron.docs: https://docs.dendron.so/
- dendron.handbook: https://handbook.dendron.so/

- NOTE: if you are a dendrologist, see additional instructions below:
    - [ ] come up with a username that they would like to have internally?
        - at Dendron, we have everyone create updates in `user.{username}` hierarchy. this lets us use @{username} syntax within notes 
        - also allows us to report progress in daily journals
        - to claim a username, create a `user.{username}` hierarchy and change the title to "{Your name}"
    - [ ] for items that we talked about in the focus area threads, add them to `user.{username}.backlog`
    - [ ] if you have any updates for the given day, you can do so in the daily note `user.kevin.journal.{date}`
        - for now, feel free to create an empty note with "hello world" to make sure things are working
        - example: [[Priorities|dendron://dendron.community/user.kevin.journal.2022.01.24#priorities]]
    - [ ] when you are done with changes, run [[Workspace Sync|dendron://dendron.dendron-site/dendron.topic.teams#workspace-sync]] to sync it together



