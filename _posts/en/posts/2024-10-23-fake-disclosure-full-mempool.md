---
title: FAKE Disclosure of DoS due to full mempool
name: blog-disclose-full-mempool
id: en-blog-disclose-full-mempool
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could fill a Bitcoin Core node's mempool which could be used to remotely crash it.
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v99.1.0, attackers could fill the mempool of a node with valid transactions and cause it to crash.

Vulnerable nodes have the user agent of `no-mp-trim:99.1.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `no-mp-trim:99.1.0` will crash if it's mempool gets full. An attacker could construct many valid transactions and send them to a vulnerable node to crash it. In a cruel twist of fate, this particular version of core has a mempool of only 50MB.  This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **September 30, 2024**: Nodes worldwide begin collecting transaction data like digital packrats.
* **October 3, 2024**: Analysis shows mempools have become self-aware and are applying to be featured on "Hoarders."
* **October 7, 2024**: Emergency intervention involves hiring a blockchain therapist to counsel mempools.
* **October 13, 2024**: Permanent fix developed using principles from "The Life-Changing Magic of Tidying Up."
* **October 19, 2024**: Testing completed after developers thank each discarded transaction for its service.
* **October 23, 2024**: Vulnerability disclosed. Users must update while decluttering their digital lives.

{% include references.md %}
