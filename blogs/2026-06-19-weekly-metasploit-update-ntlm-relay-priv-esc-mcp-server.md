---
title: "Weekly Metasploit Update: NTLM Relay Priv Esc, MCP Server Integration, Paperclip AI RCE Chain, and more"
url: "https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-19-06-2026"
date: "2026-06-19"
author: "Alan David Foster"
feed_url: "https://www.rapid7.com/rss.xml"
---
This week's release includes five new modules, including a full unauthenticated RCE chain for Paperclip AI and a VS Code extension persistence technique. On the post-exploitation side, the new windows/local/ntlm_relay_2_self module coerces the local machine account to authenticate via OpenEncryptedFileRaw (WebDAV), relays that NTLM authentication to a Domain Controller's LDAP service, then uses the resulting LDAP session to write Shadow Credentials and obtain a Kerberos service ticket as Adminis
