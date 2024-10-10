---
title: FAKE Disclosure of DoS due to unkown p2p message
name: blog-disclose-unknown-p2p
id: en-blog-disclose-unknown-p2p
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could send an unknown P2P message to a Bitcoin Core node which could be used to remotely crash it.
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v99.0.0, attackers could send an unknown P2P message which could be used to remotely crash peers.

Vulnerable nodes have the user agent of `unknown-message:99.0.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `unknown-message:99.0.0` will crash if it's sent an unknown P2P message.  This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **October 1, 2024**: Node operators report their computers speaking in tongues after receiving strange P2P messages.
* **October 3, 2024**: Developer discovers the messages are actually Klingon, sent by a Star Trek fan's malfunctioning mining rig.
* **October 5, 2024**: Team attempts to hire a Klingon translator but settles for a Trekkie convention attendee.
* **October 10, 2024**: Fix developed involving a universal translator and a tribble-based firewall.
* **October 15, 2024**: Testing delayed as all test machines keep trying to beam themselves to the Enterprise.
* **October 23, 2024**: Vulnerability disclosed. Users advised to update while wearing pointy ears for good luck.

{% include references.md %}
