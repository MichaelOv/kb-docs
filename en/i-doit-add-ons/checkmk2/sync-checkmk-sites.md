---
title: sync-checkmk-sites
description: 
published: true
date: 2025-07-02T16:11:49.880Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:11:47.628Z
---

# Sync checkmk sites

checkmk provides a distributed monitoring of hosts and its services. You can configure multiple monitoring hosts which are called "sites". To share these sites with i-doit run:

```shell
idoitcmk sync-sites
```

_Sites without hosts are not considered._

In i-doit these sites are stored in the dialog+ attribute Site in category Check_MK Host.

**Recommendation:** Run this command every time you add a new site.
