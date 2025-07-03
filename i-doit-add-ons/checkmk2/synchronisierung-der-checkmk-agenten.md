---
title: synchronisierung-der-checkmk-agenten
description: 
published: true
date: 2025-07-02T16:03:16.150Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:03:13.966Z
---

# Synchronisierung der checkmk Agenten

Checkmk bietet eine agentenbasierte Überwachung von Hosts und deren Diensten. Es gibt verschiedene Arten von Agenten, die mit i-doit geteilt werden können. Um dies zu tun, führen Sie einfach aus:

```shell
idoitcmk sync-agents
```

Dadurch werden alle verfügbaren Agententypen zu i-doit's Dialog+-Attribut "Agent" in der Kategorie Check_MK Host hinzugefügt.

**Empfehlung:** Sie müssen diesen Befehl nur einmal ausführen.
