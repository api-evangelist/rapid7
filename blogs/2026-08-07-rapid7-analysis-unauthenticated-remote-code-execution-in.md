---
title: "Rapid7 Analysis: Unauthenticated Remote Code Execution in JetBrains TeamCity (CVE-2026-63077)"
url: "https://www.rapid7.com/blog/post/ra-unauthenticated-rce-in-jetbrains-teamcity-cve-2026-63077"
date: "2026-08-07"
author: "Stephen Fewer"
feed_url: "https://www.rapid7.com/rss.xml"
---
Overview On July 27, 2026, JetBrains published a security advisory for CVE-2026-63077 , a critical unsafe deserialization vulnerability affecting JetBrains TeamCity . An attacker who can reach a TeamCity server over HTTP or HTTPS can exploit the agent polling protocol without credentials and execute operating system commands with the privileges of the TeamCity server process. JetBrains reported no known active exploitation when it disclosed the vulnerability.
