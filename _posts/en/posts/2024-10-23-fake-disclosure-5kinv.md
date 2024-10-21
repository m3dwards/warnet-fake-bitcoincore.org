---
title: FAKE Disclosure of DoS due to receiving 5k invs
name: blog-disclose-5kinv
id: en-blog-disclose-5kinv
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could crash a Bitcoin Core node by sending 5k invs
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v94.0.0, attackers could send 5000 INV messages which could be used to remotely crash peers.

Vulnerable nodes have the user agent of `k5-inv:94.0.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `5k-inv:94.0.0` will crash if it's sent 5000 INV messages. This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **October 1, 2024**: Nodes begin crashing after receiving the blockchain equivalent of a chatty neighbor's life story.
* **October 4, 2024**: Investigation reveals nodes suffering from information overload after 5000 INV messages about what other nodes had for breakfast.
* **October 8, 2024**: Temporary fix involves nodes putting their digital fingers in their ears while shouting "LA LA LA CAN'T HEAR YOU."
* **October 12, 2024**: Developers create anti-gossip filter that automatically responds "that's nice dear" to excessive INV messages.
* **October 18, 2024**: Testing successful after teaching nodes the art of setting healthy communication boundaries.
* **October 23, 2024**: Vulnerability disclosed. Users must update while wearing noise-canceling headphones and practicing mindful message acceptance.

{% include references.md %}
