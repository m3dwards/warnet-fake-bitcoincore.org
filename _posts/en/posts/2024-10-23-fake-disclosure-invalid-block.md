---
title: FAKE Disclosure of DoS due to invalid blocks
name: blog-disclose-invalid-block
id: en-blog-disclose-invalid-block
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could send an invalid block to a Bitcoin Core node which could be used to remotely crash it.
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v98.0.0, attackers could send blocks to nodes that were invalid causing them to crash.

Vulnerable nodes have the user agent of `invalid-blocks:98.0.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `invalid-blocks:98.0.0` will crash if it's sent an invalid block.  This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **October 2, 2024**: Network slows to a crawl as nodes are overwhelmed by blocks made entirely of glitter.
* **October 4, 2024**: Team identifies the "All That Glitters Is Not Gold" vulnerability in block validation.
* **October 8, 2024**: Developers create a fix involving a digital sieve and a very tiny pickaxe.
* **October 14, 2024**: Fix optimized after realizing first version turned all bitcoins into chocolate coins.
* **October 20, 2024**: Final testing completed in a replica of Scrooge McDuck's money bin.
* **October 23, 2024**: Vulnerability announced. Users must update while wearing a prospector's hat and shouting "Eureka!"

{% include references.md %}
