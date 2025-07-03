---
title: wato-ordner-synchronisieren
description: 
published: true
date: 2025-07-02T16:03:25.318Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:03:23.067Z
---

# WATO Ordner synchronisieren

Hosts können hierarchisch in Ordnern geordnet werden. Diese Ordner können mit i-doit synchronisiert werden und zusätzliche Ordner in i-doit können verwendet werden, um neue Ordner in Check\_MK zu erstellen. Einfach ausführen:

```shell
idoitcmk sync-folders
```

In i-doit werden diese WATO-Ordner im Dialog+-Attribut WATO-Ordner in der Kategorie Check_MK Host gespeichert.

**Empfehlung:** Führen Sie diesen Befehl jedes Mal aus, wenn Sie einen neuen Ordner in checkmk oder i-doit hinzufügen.
