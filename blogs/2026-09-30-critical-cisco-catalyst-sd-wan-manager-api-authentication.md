---
title: "Critical Cisco Catalyst SD-WAN Manager API authentication bypass exploited in the wild (CVE-2026-76504)"
url: "https://www.rapid7.com/blog/post/etr-critical-cisco-catalyst-sd-wan-manager-api-authentication-bypass-exploited-in-the-wild-cve-2026-76504"
date: "2026-09-30"
author: "Rapid7"
feed_url: "https://www.rapid7.com/rss.xml"
---
Overview On September 30, 2026, Cisco published a security advisory for CVE-2026-76504 , a critical API authentication bypass vulnerability affecting Cisco Catalyst SD-WAN Manager. The vulnerability has a CVSSv3.1 score of 9.8 and results from improper handling of URL encoding ( CWE-177 ). An unauthenticated, remote attacker can send a crafted HTTP request that bypasses an authentication rule for a specific API endpoint, gaining access to the API with the privileges of the admin user.
