---
title: checkmk-sites-synchronisieren
description: 
published: true
date: 2025-07-02T16:02:40.924Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:02:38.593Z
---

# checkmk sites synchronisieren

checkmk bietet eine verteilte Überwachung von Hosts und deren Diensten. Sie können mehrere Überwachungshosts konfigurieren, die als "Sites" bezeichnet werden. Um diese Sites mit i-doit zu teilen, führen Sie aus:

```shell
idoitcmk sync-sites
```

\*Sites ohne Hosts werden nicht berücksichtigt.

In i-doit werden diese Sites im Dialog+ Attribut Site in der Kategorie Check_MK Host gespeichert.

**Empfehlung:** Führen Sie diesen Befehl jedes Mal aus, wenn Sie eine neue Site hinzufügen.
