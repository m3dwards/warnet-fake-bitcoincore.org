---
title: FAKE Disclosure of DoS due to orphan spam
name: blog-disclose-orphan-spam
id: en-blog-disclose-orphan-spam
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could send over 50 orphans to a Bitcoin Core node which could be used to remotely crash it.
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v99.1.0, attackers could spam nodes with over 50 orphan transactions which could be used to remotely crash peers.

Vulnerable nodes have the user agent of `50-orphans:99.1.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `50-orphans:99.1.0` will crash if it's sent over 50 orphan transactions.  This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **September 28, 2024**: Mining pools crash after millions of transactions appear asking for "more porridge, please."
* **October 1, 2024**: Investigation reveals attackers exploiting nodes' sympathy for orphaned transactions.
* **October 5, 2024**: Temporary fix involves nodes singing "It's a Hard Knock Life" to repel excessive orphans.
* **October 12, 2024**: Permanent solution developed: each node adopts a limited number of orphan transactions.
* **October 18, 2024**: Testing completed using a blockchain-based production of "Annie."
* **October 23, 2024**: Vulnerability disclosed. Users must update while wearing a curly red wig.

{% include references.md %}
