---
title: mysql-server-has-gone-away
description: 
published: true
date: 2025-07-02T16:16:42.768Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:16:39.977Z
---

# "MySQL-Server Has Gone Away"

Problem
-------

When starting i-doit the error message "MySQL-Server has gone away" appears.

Solution
--------

The default configuration of the property ***max_allowed_packet*** has the value 1M in some environments. Adjust this setting in the configuration file of MySQL/MariaDB as follows:

    max_allowed_packet = 128M

Also take a look at our recommended [system settings](../../installation/manual-installation/system-settings.md).