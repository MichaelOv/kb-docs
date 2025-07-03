---
title: sync-wato-folder
description: 
published: true
date: 2025-07-02T16:11:59.752Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:11:57.590Z
---

# Sync WATO folders

Hosts can be hierarchical ordered in folders. These folders can be synced to i-doit and additional folders in i-doit can be used to generate new folders in checkmk. Just run:

```shell
idoitcmk sync-folders
```

In i-doit these WATO folders are stored in the dialog+ attribute WATO folder in category Check_MK Host.

**Recommendation:** Run this command every time you add a new folder in checkmk or i-doit.
